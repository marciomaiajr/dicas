# Markdown

## Markdown mode no emacs

[https://www.markdownguide.org/basic-syntax/](https://www.markdownguide.org/basic-syntax/)

tl;dr

Para Instalar o modo markdown no emacs, inserir o código abaixo no init.el

``` emacs-lisp
(use-package markdown-mode
  :ensure t
  :commands (markdown-mode gfm-mode)
  :mode (("README\\.md\\'" . gfm-mode)
         ("\\.md\\'" . markdown-mode)
         ("\\.markdown\\'" . markdown-mode)))
```
