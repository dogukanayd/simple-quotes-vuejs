<template>
    <div class="row">
        <div class="col-sm-12">
            <h3>Quotes Added</h3>
            <div class="progress">
                <div class="progress">
                    <div class="progress-bar" role="progress-bar" aria-valuenow="60" aria-volumein="0" aria-volumemax="100"
                    :style="{width: (quoteCount / maxQoutes) * 100 + '%'}">
                        {{ quoteCount }} / {{ maxQoutes }}
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default{
        props: ['quoteCount', 'maxQoutes']
    }
</script>
