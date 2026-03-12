# New Laptop Setup Prompt for Web Claude

Copy and paste everything below the line into Web Claude on your new laptop:

---

I need help setting up my new Windows laptop for coding. I'm new to coding so please walk me through each step clearly.

Here's what I need installed in this order:

1. **WSL2 (Windows Subsystem for Linux)**
   - Open PowerShell as Administrator
   - Run: wsl --install
   - Restart the laptop when prompted
   - After restart, open Ubuntu from Start menu and create a username and password

2. **VS Code**
   - Download and install VS Code from https://code.visualstudio.com
   - Once installed, open VS Code and install the "WSL" extension (by Microsoft)
   - Connect VS Code to WSL: click the blue >< icon in the bottom-left corner and select "Connect to WSL"

3. **Git** (inside WSL/Ubuntu terminal)
   - sudo apt update && sudo apt install git -y

4. **Python 3** (inside WSL/Ubuntu terminal)
   - sudo apt install python3 python3-pip -y

5. **Node.js via nvm** (inside WSL/Ubuntu terminal)
   - curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.1/install.sh | bash
   - Close and reopen the terminal
   - nvm install --lts

6. **Claude Code** (inside WSL/Ubuntu terminal)
   - npm install -g @anthropic-ai/claude-code
   - Run: claude
   - Log in with my Anthropic account when prompted

Once Claude Code is running in the WSL terminal, I'm all set. Claude Code will handle the rest (git config, SSH keys, cloning my repos, installing tools and extensions).

Please walk me through each step one at a time and wait for me to confirm before moving to the next one.
