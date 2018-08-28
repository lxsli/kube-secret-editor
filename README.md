# Edit Kubernetes secrets

Usage:

    $> KUBE_EDITOR=/path/to/kube-secret-editor.py kubectl edit secret my-secret

This fork is for noninteractive secret editing. The script will:
- read ~/.ksecretvals
- read the secret
- merge that into the secret, encoding to b64 as it goes
- write the secret
