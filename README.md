Arquivo index inicial apenas para referências o link para os dois caminhos abaixo citados:

Pasta PAC/ para preechimento e registro dos dados dos pacientes. -> Gera um PDF de acordo com o que foi registrado. PDF salvo no (Firebase - Storage)
Pasta ENF/ para pesquisar por Nome ou Código do Convênio o paciente registado. -> Consulta e mostra campos salvos no (Firebase - Firestore Database) incluso arquivos anexados, PDF gerado.

Bootstrap 4.5.2 para Estilo da página:
  <link href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" rel="stylesheet">

Material Icons do Google atualmente com dois ícones utilizados:
  <link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">

Criação do PDF:
  <script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.3.1/jspdf.umd.min.js"></script>


Imports para inicialização do Storage e Firestore Database do Firebase:

    import { initializeApp } from "https://www.gstatic.com/firebasejs/9.0.0/firebase-app.js";
    import { getFirestore, collection, addDoc, Timestamp } from "https://www.gstatic.com/firebasejs/9.0.0/firebase-firestore.js";
    import { getStorage, ref, uploadBytes, getDownloadURL } from "https://www.gstatic.com/firebasejs/9.0.0/firebase-storage.js";

