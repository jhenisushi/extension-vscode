# GeneXus 8 Support (VS Code Extension)

Extensão para o Visual Studio Code que adiciona **suporte básico à linguagem GeneXus 8**:

- **Realce de sintaxe** (keywords, funções, variáveis, atributos, comentários, etc.)
- **Snippets** para estruturas comuns (`If/EndIf`, `For Each/EndFor`, `Sub/EndSub`, ...)
- **Tema dedicado** com cores harmonizadas (estilo Dark+/C-like)
- **Indentação básica** (abertura/fechamento de blocos)

---

## Instalação (local)

1. Clone este repositório:
   ```bash
   git clone https://github.com/seuusuario/genexus8-support.git
   cd genexus8-support
````

2. Empacote a extensão:

   ```bash
   vsce package
   ```

   Isso gera um arquivo `.vsix`.

3. Instale no VS Code:

   * Método gráfico:
     `Ctrl+Shift+P` → `Extensions: Install from VSIX` → escolha o `.vsix`
   * Método CLI:

     ```bash
     code --install-extension genexus8-support-0.0.3.vsix
     ```

4. Abra um arquivo `.gx`, `.prc`, `.src`, `.prg` ou `.gx8` → a coloração deve ser aplicada.

---

## Uso

* Crie arquivos com extensões reconhecidas (`.gx`, `.prc`, `.src`, `.prg`, `.gx8`).
* A extensão aplica:

  * **Cores** para keywords, variáveis, funções GeneXus, atributos de banco e comentários.
  * **Snippets**: digite `if`, `foreach`, `sub` e pressione `Tab` para expandir.
  * **Indentação** automática em blocos (`If/EndIf`, `For Each/EndFor`, etc.).

---

## Roadmap

* [x] Syntax highlighting
* [x] Tema dedicado
* [x] Snippets básicos
* [ ] Formatter (alinhamento automático, estilo Prettier)
* [ ] Melhorar auto-complete de variáveis/atributos
* [ ] Publicar no Marketplace

---

## Contribuição

Pull requests são bem-vindos!
Sugestões de novas keywords/funções também. Abra uma **issue** ou envie um PR com a modificação no arquivo `syntaxes/genexus8.tmLanguage.json`.
