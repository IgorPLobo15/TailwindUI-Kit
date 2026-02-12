# Tailwind UI Kit

Kit de componentes Tailwind UI em múltiplas versões: HTML, Alpine.js, React e Vue. Inclui um preview para visualizar os componentes no navegador.

## Estrutura do projeto

| Pasta      | Descrição                          |
|-----------|-------------------------------------|
| `preview/` | Aplicação para visualizar os componentes |
| `html/`    | Componentes em HTML puro            |
| `alpine/`  | Componentes com Alpine.js           |
| `react/`   | Componentes em React (JSX)          |
| `vue/`     | Componentes em Vue                  |

## Como rodar o projeto

O preview é um site estático. Você precisa de um servidor HTTP local (não basta abrir o `index.html` direto no navegador).

### Pré-requisito

- [Node.js](https://nodejs.org/) (qualquer versão LTS)

### Passos

1. Abra o terminal na raiz do projeto:

   ```bash
   cd caminho/para/TailwindUI-Kit
   ```

2. Inicie o servidor na pasta `preview`:

   ```bash
   npx serve preview -l 3000
   ```

   - `npx serve` sobe um servidor estático (não precisa instalar nada antes).
   - `preview` é a pasta que será servida.
   - `-l 3000` define a porta 3000 (opcional; sem isso o `serve` usa outra porta).

3. Acesse no navegador:

   - **http://localhost:3000**

   A página inicial redireciona automaticamente para **http://localhost:3000/components/**, onde ficam os componentes para visualização.

### Parar o servidor

No terminal onde o servidor está rodando, pressione **Ctrl+C**.

### Usar outra porta

Para usar outra porta (por exemplo 8080):

```bash
npx serve preview -l 8080
```

Depois acesse **http://localhost:8080**.

---

**Resumo:** na raiz do projeto, execute `npx serve preview -l 3000` e abra http://localhost:3000 no navegador.
