<template>
    <div>
        <h1>{{pageName}}</h1>
        <p>{{pageDescription}}</p>

    </div>

</template>
<script>
    export default {

        data: function () {
            return {
                pageName: "help us",
                pageDescription: "this is help page"
            };

        },
        name: 'help'

    };

</script>