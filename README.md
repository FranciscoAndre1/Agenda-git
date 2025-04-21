// agenda de contatos
let contatos = [];

function adicionarContato() {
    let nome = prompt("Digite o nome do contato:");
    let telefone = prompt("Digite o telefone do contato:");
    let email = prompt("Digite o email do contato:");

    let contato = {
        nome: nome,
        telefone: telefone,
        email: email
    };

    contatos.push(contato);
    console.log("Contato adicionado com sucesso!");

    exibirContatos();
    adicionarContato();
}

function exibirContatos() {
    console.log("Contatos:");
    for (let i = 0; i < contatos.length; i++) {
        let contato = contatos[i];
        console.log(`Nome: ${contato.nome}`);
        console.log(`Telefone: ${contato.telefone}`);
        console.log(`Email: ${contato.email}`);
        console.log("--------------------");
    }
}   
exibirContatos();
adicionarContato();
