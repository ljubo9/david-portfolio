<script>


export default {
    data() {
        return {
            currentYear: new Date().getFullYear(),
        }
    }
}


</script>

<template>

<hr>

<div class="d-flex justify-content-center align-items-center">
    <p class="text-sm mt-2 opacity-50">
		&copy; {{currentYear}} David Ljubić. All rights reserved.
    </p>
</div>
  
</template>

