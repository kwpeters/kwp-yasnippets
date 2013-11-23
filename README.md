kwp-yasnippets
==============

This is my collection of custom yasnippets.

# Configuration

Add the following to .emacs:

```
;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
;;
;; yasnippet
;;
;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;

(setq yas-snippet-dirs
      '("~/kwp/appdata/emacs/yasnippet/kwp-yasnippets"        ;; personal snippets
        ;;"~/kwp/appdata/emacs/yasnippet/default-snippets"    ;; the default collection
        ))

(add-hook 'sgml-mode-hook
          '(lambda ()
             (yas-minor-mode)
             (yas-reload-all)
             )
          )

(add-hook 'js2-mode-hook
          '(lambda ()
             (yas-minor-mode)
             (yas-reload-all)
             )
          )
```
