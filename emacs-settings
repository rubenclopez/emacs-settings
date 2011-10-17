;;;;;;;;;;;;
;;js yeggi;;
;;;;;;;;;;;;
(add-to-list 'load-path "~/.emacs.d/js")
(autoload 'js2-mode "js2" nil t)
(add-to-list 'auto-mode-alist '("\\.js$" . js2-mode))


;;;;;;;;;;;;
;;textmate;;
;;;;;;;;;;;;
(add-to-list 'load-path "~/.emacs.d/textmate")
(require 'textmate)
(textmate-mode)

;;;;;;;;;;;;;
;;YaSnippet;;
;;;;;;;;;;;;;
 (add-to-list 'load-path
                  "~/.emacs.d/yasnippet")
    (require 'yasnippet) ;; not yasnippet-bundle
    (yas/initialize)
    (yas/load-directory "~/.emacs.d/yasnippet")

;;;;;;;;;
;;theme;;
;;;;;;;;;
(require 'color-theme)
(color-theme-initialize)
(load-file "~/.emacs.d/themes/color-theme-twilight.el")
(color-theme-twilight)

;;;;;;;;;;;;;;;;
;;Transparency;;
;;;;;;;;;;;;;;;;
 (set-frame-parameter (selected-frame) 'alpha '(85 80))
 (add-to-list 'default-frame-alist '(alpha 85 80))

;;;;;;;;;;;;
;;SoftTabs;;
;;;;;;;;;;;;
(add-hook 'write-file-hooks 
          (lambda () (if (not indent-tabs-mode)
                         (untabify (point-min) (point-max)))))
 (setq-default indent-tabs-mode nil)

;; adding ruby electric
(add-hook 'ruby-mode-hook
          (lambda()
            ;;          (add-hook 'local-write-file-hooks
            ;;                    '(lambda()
            ;;                       (save-excursion
            ;;                         (untabify (point-min) (point-max))
            ;;                         (delete-trailing-whitespace)
            ;;                         )))
            ;;          (set (make-local-variable 'indent-tabs-mode) 'nil)
            ;;          (set (make-local-variable 'tab-width) 2)
            (imenu-add-to-menubar "IMENU")
            (define-key ruby-mode-map "\C-m" 'newline-and-indent)
            ;;          (require 'ruby-electric)
            ;;          (ruby-electric-mode t)
            ))
(put 'downcase-region 'disabled nil)

;;;;;;;;;;;;;
;;TAB STOPS;;
;;;;;;;;;;;;;


(custom-set-variables
  ;; custom-set-variables was added by Custom.
  ;; If you edit it by hand, you could mess it up, so be careful.
  ;; Your init file should contain only one such instance.
  ;; If there is more than one, they won't work right.
 '(tab-stop-list (quote (2 4 6 8 10 12 14 16 18 20 22 24 26 28 30 32 34 36 38 40 42 44 46 48 50 52 54 56 58 60 62 64 66 68 70 72 74 76 78 80 82 84 86 88 90 92 94 96 98 100 102 104 106 108 110 102 104 106 108 110 112 114 116 118 120))))
(custom-set-faces
  ;; custom-set-faces was added by Custom.
  ;; If you edit it by hand, you could mess it up, so be careful.
  ;; Your init file should contain only one such instance.
  ;; If there is more than one, they won't work right.
 )