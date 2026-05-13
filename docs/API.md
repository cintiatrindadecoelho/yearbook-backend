import express from "express";

const app = express();

app.get("/usuarios", (req, res) => {
  res.status(200).json({
    mensagem: "Lista de usuários"
  });
});

app.post("/usuarios", (req, res) => {
  res.status(201).json({
    mensagem: "Usuário criado"
  });
});

app.listen(3000);