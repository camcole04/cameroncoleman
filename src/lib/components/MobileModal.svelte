<script>
    import { onMount } from 'svelte';
    
    let showModal = false;
    
    onMount(() => {
        // check if device is mobile based on screen width
        const checkMobile = () => {
            const isMobile = window.innerWidth <= 768;
            if (isMobile) {
                // check if user has already seen the modal
                const hasSeenModal = localStorage.getItem('mobileModalSeen');
                if (!hasSeenModal) {
                    showModal = true;
                }
            }
        };
        
        checkMobile();
        window.addEventListener('resize', checkMobile);
        
        return () => {
            window.removeEventListener('resize', checkMobile);
        };
    });
    
    function closeModal() {
        showModal = false;
        localStorage.setItem('mobileModalSeen', 'true');
    }
    
    function handleBackdropClick(event) {
        if (event.target === event.currentTarget) {
            closeModal();
        }
    }
    
    function handleKeyDown(event) {
        if (event.key === 'Escape' || event.key === 'Enter' || event.key === ' ') {
            event.preventDefault();
            closeModal();
        }
    }
</script>

{#if showModal}
    <div 
        class="modal-backdrop" 
        role="dialog"
        aria-modal="true"
        aria-labelledby="modal-title"
        on:click={handleBackdropClick}
        on:keydown={handleKeyDown}
        tabindex="-1"
    >
        <div class="modal-content">
            <div class="modal-header">
                <h2 id="modal-title">📱 Mobile Notice</h2>
            </div>
            <div class="modal-body">
                <p>
                    Hey! The site looks pretty bad on smaller devices. Sorry about that! 
                    It will be fixed eventually, feel free to explore it anyway. 
                    Thank you!
                </p>
            </div>
            <div class="modal-footer">
                <button class="continue-btn" on:click={closeModal}>
                    Continue Anyway
                </button>
            </div>
        </div>
    </div>
{/if}

<style>
    .modal-backdrop {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background-color: rgba(0, 0, 0, 0.7);
        display: flex;
        justify-content: center;
        align-items: center;
        z-index: 1000;
        animation: fadeIn 0.3s ease-in-out;
    }

    .modal-content {
        background-color: #f5f1e9;
        border-radius: 15px;
        padding: 30px;
        max-width: 90%;
        width: 400px;
        box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
        animation: slideIn 0.3s ease-out;
        border: 3px solid #d2b48c;
    }

    .modal-header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-bottom: 20px;
        border-bottom: 2px solid #d2b48c;
        padding-bottom: 10px;
    }

    .modal-header h2 {
        margin: 0;
        color: #8b4513;
        font-family: 'Georgia', serif;
        font-size: 24px;
    }

    .modal-body {
        margin-bottom: 20px;
    }

    .modal-body p {
        margin: 0;
        color: #5a3e1b;
        font-family: 'Georgia', serif;
        font-size: 16px;
        line-height: 1.6;
        text-align: center;
    }

    .modal-footer {
        text-align: center;
    }

    .continue-btn {
        background-color: #8b4513;
        color: white;
        border: none;
        padding: 12px 30px;
        border-radius: 25px;
        font-family: 'Georgia', serif;
        font-size: 16px;
        cursor: pointer;
        transition: background-color 0.3s ease;
    }

    @keyframes fadeIn {
        from {
            opacity: 0;
        }
        to {
            opacity: 1;
        }
    }

    @keyframes slideIn {
        from {
            transform: translateY(-50px);
            opacity: 0;
        }
        to {
            transform: translateY(0);
            opacity: 1;
        }
    }

    @media (max-width: 480px) {
        .modal-content {
            margin: 20px;
            padding: 20px;
        }
        
        .modal-header h2 {
            font-size: 20px;
        }
        
        .modal-body p {
            font-size: 14px;
        }
    }
</style>
