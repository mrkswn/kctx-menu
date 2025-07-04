# `kctx-menu`

Bash helper that lists each Kubernetes context in your `kubeconfig` and lets you switch by entering the corresponding number.

```
Available contexts:
[1] arn:aws:eks:us-west-2:123456789012:cluster/dev
[2] arn:aws:eks:us-west-2:123456789012:cluster/staging
[3] docker-desktop
[4] kind-kind

Choose a context by number: 2
Switched to "arn:aws:eks:us-west-2:123456789012:cluster/staging".
✅  Now using context: arn:aws:eks:us-west-2:123456789012:cluster/staging
```
## Installation

```bash
# Download script
curl -Lo kctx-menu https://raw.githubusercontent.com/mrkswn/kctx-menu/main/kctx-menu
chmod +x kctx-menu

# Put it in PATH
mv kctx-menu ~/bin/     # or /usr/local/bin, ~/.local/bin, etc.

# Add as an alias
echo 'alias km="kctx-menu"' >> ~/.bashrc     # or ~/.zshrc
source ~/.bashrc

# Usage
km     # or kctx-menu
```
