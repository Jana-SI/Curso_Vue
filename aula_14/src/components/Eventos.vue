<template>
    <form action="" @submit="enviarForm($event)">

        <div class="row mb-3">
            <div class="col-12">
                <input type="text" class="form-control" v-model="name" placeholder="Digite o seu nome"
                    aria-label="Digite o seu nome">
            </div>
        </div>

        <div class="row mb-3">
            <div class="col-12">
                <input type="text" class="form-control" v-model="email" placeholder="email@email"
                    aria-label="email@email">
            </div>
        </div>

        <div class="row mb-3 align-items-center justify-content-center">
            <div class="col-6 text-center">
                <button class="btn " type="submit">Enviar</button>
            </div>
        </div>
    </form>

    <p class="card-text border-top border-white">
        Data Binding<br>
       Nome: <span><strong>{{ name }}</strong></span><br>
       E-mail: <span><strong>{{ email }}</strong></span>
    </p>
    <p class="card-text border-top border-white">
        Por submit<br>
        Nome: <span><strong>{{ input_name }}</strong></span><br>
       E-mail: <span><strong>{{ input_email }}</strong></span>
    </p>
</template>

<script>

export default {
    name: 'Eventos',
    data() {
        return {
            name: "",
            email: "",
            input_name: "",
            input_email: ""
        }
    },
    methods: {
        enviarForm(e) {
            e.preventDefault();

            const name = this.name;
            const email = this.email;

            this.input_name = this.name;
            this.input_email = this.email;

            console.log("Formulário Enviado");
            console.log("Nome: " + name);
            console.log("Email: " + email);
        }
    }
}

</script>

<style scoped>
form {
    padding: 10px;
}

input {
    padding: 10px;
}

.btn {
    background-color: #37495f !important;
    color: white !important;
    border: 2px solid white;
}

.btn:hover {
    background-color: white !important;
    color: #37495f !important;
    border: 2px solid #37495f !important;
}
</style>