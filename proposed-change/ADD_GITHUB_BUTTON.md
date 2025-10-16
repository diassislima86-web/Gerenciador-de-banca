# Proposta: Adicionar botão "Abrir no GitHub" no cabeçalho

Proponho adicionar um botão no cabeçalho da página principal (arquivo: `Gerenciador`) para facilitar o acesso ao repositório do projeto.

Onde inserir:
- Inserir logo após a tag `<h1>` dentro do elemento `<header class="text-center p-6 card">`.

Trecho HTML sugerido (colar exatamente após o `<h1>`):

```html
<!-- Botão adicionado: abre o repositório do projeto em nova aba -->
<div class="mt-3">
    <button
        onclick="window.open('https://github.com/diassislima86-web/Gerenciador-de-banca', '_blank', 'noopener')"
        aria-label="Abrir repositório no GitHub"
        class="inline-flex items-center gap-2 ml-auto py-2 px-4 rounded bg-indigo-600 text-white hover:bg-indigo-700 shadow-sm transition"
    >
        Abrir no GitHub
    </button>
</div>
```

Notas:
- O botão usa `window.open` com `noopener` por segurança e `aria-label` para acessibilidade.
- Posso aplicar diretamente a modificação no arquivo `Gerenciador` em um commit separado se você aprovar esta proposta.

Obrigado!