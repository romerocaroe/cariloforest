<template>
    <v-form ref="form" autocomplete="off" @submit.prevent="save">
        <v-row>
            
            <v-col cols="12" sm="12">
                <h4 v-t="'people.person.main'"></h4>
            </v-col>

            <v-col cols="12" sm="6">
                <v-text-field
                    prepend-icon="account_box"
                    name="name"
                    type="text"
                    v-model="form.name"
                    :label="$t('people.person.name')"
                    :placeholder="$t('people.person.name')"
                    class="pa-3"
                    :rules="requiredAlphabeticApostropheCharacters"
                    :error="hasInputErrors('name')"
                    :error-messages="getInputErrors('name')"
                    required
                    color="secondary"
                ></v-text-field>
            </v-col>

            <v-col cols="12" sm="6">
                <v-text-field
                        prepend-icon="account_box"
                        name="lastname"
                        type="text"
                        v-model="form.lastname"
                        :label="$t('people.person.lastname')"
                        :placeholder="$t('people.person.lastname')"
                        class="pa-3"
                        :rules="requiredAlphabeticApostropheCharacters"
                        :error="hasInputErrors('lastname')"
                        :error-messages="getInputErrors('lastname')"
                        required
                        color="secondary"
                ></v-text-field>
            </v-col>

        </v-row>
    </v-form>
</template>

<script>
   export default {
    name: "GuestForm",
    data(){
      return {
        guests: ["uno","dos","tres"]
      }
    },
    computed: {
        form: {
            get() {
                return this.value;
            },
            set(val) {
                this.$emit("input", val);
            },
        },
    }
  }
</script>

<style scoped>
</style>