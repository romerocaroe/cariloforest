<template>
    <v-container fluid>
        <Header></Header>
        <guestCreate></guestCreate>
    </v-container>
</template>

<script>
import Header from '../Layout/Header';
import GuestCreate from './GuestCreate';

export default {
    name: "GuestMain",
    components: {
        Header,
        GuestCreate
    }
}
</script>

<style scoped>

</style>