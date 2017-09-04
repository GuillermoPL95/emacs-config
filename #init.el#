;;; package:
;;; code:
(ido-mode)

(global-linum-mode 1)
(require 'package)
(add-to-list 'package-archives
             '("marmalade" . "http://marmalade-repo.org/packages/"))
(add-to-list 'package-archives
             '("melpa"."http://melpa.org/packages/"))
(add-to-list 'package-archives
             '("elpy" . "http://jorgenschaefer.github.io/packages/"))
(package-initialize)
(custom-set-variables
 ;; custom-set-variables was added by Custom.
 ;; If you edit it by hand, you could mess it up, so be careful.
 ;; Your init file should contain only one such instance.
 ;; If there is more than one, they won't work right.
 '(custom-safe-themes
   (quote
    ("70403e220d6d7100bae7775b3334eddeb340ba9c37f4b39c189c2c29d458543b" default)))
 '(inhibit-startup-screen t))
(custom-set-faces
 ;; custom-set-faces was added by Custom.
 ;; If you edit it by hand, you could mess it up, so be careful.
 ;; Your init file should contain only one such instance.
 ;; If there is more than one, they won't work right.
 )

(add-to-list 'load-path
              "~/.emacs.d/plugins/yasnippet")
(require 'yasnippet)
(yas-global-mode 1)
(require 'ox-reveal)
(add-hook 'fancy-diary-display-mode-hook
          '(lambda ()
             (alt-clean-equal-signs)))

(setq org-reveal-root "/home/guillermo/reveal.js")

(load-theme 'darkokai t)
;use package:

;(use-package ensime
;  :ensure t
;  :pin melpa-stable)
;; To quit the auto backups archives
(setq backup-directory-alist '(("." . "~/.emacs.d/backups/")))

;; Package Flycheck
(require 'package)
(add-to-list 'package-archives
             '("MELPA Stable" . "http://stable.melpa.org/packages/") t)
(package-initialize)
(package-refresh-contents)

(package-install 'flycheck)

(global-flycheck-mode)
(add-hook 'after-init-hook #'global-flycheck-mode)

;;; elpy

(setq elpy-rpc-python-command "python3")
(package-initialize)
(elpy-enable)

;;; init.el ends here
