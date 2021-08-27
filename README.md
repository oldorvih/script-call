# script-call
Script bd
CREATE TABLE login_ast (
  login_id SERIAL,
  nome varchar(30) NOT NULL,
  login integer NOT NULL,
  senha integer NOT NULL,
  contexto varchar(30) NOT NULL,
  CONSTRAINT login_ast_pk PRIMARY KEY (nome, login, senha, contexto),
  CONSTRAINT login_ast_idx UNIQUE (login)
);

COMMENT ON TABLE login_ast IS 'Tabela do Asterisk de senhas para realizar ligacoes';
