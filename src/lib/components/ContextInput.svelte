<script lang="ts">
export let additionalContext = ''
</script>

<details class="context-details">
    <summary>Add more context</summary>
    <textarea
        class="context-input"
        rows="4"
        bind:value={additionalContext}
        placeholder="Anything else we should know about?"
    ></textarea>
</details>

<style>
    details.context-details {
        text-align: left;
        border: 1px solid var(--light);
        background-color: var(--white);
        margin-right: 1rem;
        border-radius: var(--border-radius);
        padding: 1rem;
        margin-bottom: 1rem;
        box-shadow: 0 2px 4px rgba(0, 0, 0, 0.05);
    }

    details summary {
        cursor: pointer;
        font-weight: 500;
        /* Using the browser's default disclosure triangle */
    }

    textarea.context-input {
        width: 90%;
        margin-top: 0.75rem;
        padding: 0.75rem;
        border: 1px solid var(--light);
        border-radius: var(--border-radius);
        resize: vertical;
        font-size: 16px; /* Prevents iOS zoom on focus */
        min-height: 80px;
    }
    
    @media (min-width: 768px) {
        details.context-details {
            padding: 1.25rem;
        }
    }
</style>
