# Catalogo de Cores

Um catalogo visual e pesquisável com **539 cores**, feito com HTML, CSS e JavaScript puro.

O projeto carrega as cores a partir de `colors.json` e monta uma grade responsiva com amostras, nomes e códigos hexadecimais. E uma forma simples de consultar paletas, descobrir nomes de cores e copiar referencias para projetos visuais.

## Previa

Ao abrir `index.html`, voce encontra:

- grade responsiva de cores;
- busca por nome ou código hexadecimal;
- contador de resultados filtrados;
- contraste automático no texto de cada amostra;
- interface leve, sem dependências externas.

## Estrutura

```text
Color_Catalog/
+-- colors.html   # Interface do catalogo
+-- colors.json   # Lista de cores em formato JSON
+-- LICENSE       # Licença AGPL-3.0
`-- README.md     # Documentação do projeto
```

## Como Usar

Como a pagina usa `fetch("colors.json")`, abra o projeto por um servidor local para garantir que o JSON seja carregado corretamente.

Com Python:

```bash
python -m http.server 8000
```

Depois acesse:

```text
http://localhost:8000/index.html
```

Também e possível usar qualquer servidor estático, como Live Server no VS Code.

## Formato Das Cores

Cada cor em `colors.json` segue este formato:

```json
{
  "hex": "AB274F",
  "name": "Rosa Cereja"
}
```

Campos:

- `hex`: código hexadecimal da cor, sem `#`;
- `name`: nome exibido no catalogo.

## Editando O Catalogo

Para adicionar uma nova cor, inclua um novo objeto em `colors.json`:

```json
{
  "hex": "4B7BEC",
  "name": "Azul Sereno"
}
```

Depois recarregue a pagina. A nova cor aparecera automaticamente na grade e tambem podera ser encontrada pela busca.

## Tecnologias

- HTML semântico;
- CSS responsivo;
- JavaScript puro;
- JSON como fonte de dados.

## Ideias Para Evoluir

- botão para copiar o código hexadecimal;
- filtros por famílias de cor;
- suporte a favoritos;
- exibição em RGB, HSL e CMYK;
- modo escuro.

## Licença

Este projeto esta licenciado sob a **GNU Affero General Public License v3.0**.

Consulte o arquivo [LICENSE](LICENSE) para mais detalhes.
