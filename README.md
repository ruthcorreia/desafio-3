class Heroi {
    constructor(nome, idade, tipo) {
        this.nome = nome;
        this.idade = idade;
        this.tipo = tipo;
    }

    atacar() {
        let ataque;
        
        // Define o ataque conforme o tipo do herói
        if (this.tipo === "mago") {
            ataque = "magia";
        } else if (this.tipo === "guerreiro") {
            ataque = "espada";
        } else if (this.tipo === "monge") {
            ataque = "artes marciais";
        } else if (this.tipo === "ninja") {
            ataque = "shuriken";
        } else {
            ataque = "ataque desconhecido"; // Caso o tipo seja outro
        }

        console.log(`O ${this.tipo} atacou usando ${ataque}`);
    }
}

// Exemplos de uso:
const heroi1 = new Heroi("Gandalf", 1000, "mago");
heroi1.atacar(); // Saída: O mago atacou usando magia

const heroi2 = new Heroi("Arthur", 35, "guerreiro");
heroi2.atacar(); // Saída: O guerreiro atacou usando espada

const heroi3 = new Heroi("Aang", 17, "monge");
heroi3.atacar(); // Saída: O monge atacou usando artes marciais

const heroi4 = new Heroi("Naruto", 20, "ninja");
heroi4.atacar(); // Saída: O ninja atacou usando shuriken
