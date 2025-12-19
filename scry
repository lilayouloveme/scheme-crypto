(require crypto)
(require crypto/libcrypto)

(define key (generate-cipher-key '(aes gcm)))
(define iv (generate-cipher-iv '(aes gcm)))
(define ct (encrypt '(aes gcm) key iv #"Nevermore!" #:aad #"quoth the raven"))
(decrypt '(aes gcm) key iv ct #:aad #"quoth the raven")
