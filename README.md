
# DevOps - TP1: Mastering Git

🚀 Welcome to DevOps TP1! 

**Part 1 - Setting Up Git Environment**:

1. **Generating an SSH Key** 🛡️
   - Generate an SSH key with the command:
     ```
     ssh-keygen -t rsa -b 4096 -C your.email@example.com
     ```
   - Copy the SSH public key using:
     ```
     cat ~/.ssh/id_rsa.pub
     ```
   - Connect to your remote repository (e.g., GitHub) and add the SSH public key in account settings.

2. **Configuring Git** ⚙️
   - Configure the name and email for proper identification in commits with:
     ```
     git config --global user.name "Your Name"
     git config --global user.email your@email.com
     ```

3. **SSH Connection to Remote Repositories** 🔗
   - Test the SSH connection using the following command. Be sure to replace `git@github.com` with the address of the remote server where repositories will be hosted:
     ```
     ssh -T git@github.com
     ```
   - Alternatively, use:
     ```
     ssh -T git@gitlab.com
     ```

**Part 2 - Creating a New Project**:

1. **Accessing Your GitHub (or GitLab) Account** 📂
   - Log in to your GitHub (or GitLab) account.
   - After logging in, select the "New" button to create a new project.
   - Give it a meaningful name and choose the appropriate options (public or private, with or without a README, etc.), then click "Create Repository" (or "Create Repository").

2. **Recording the Project's URL** 🔗
   - The URL will appear like this: `git@github.com:your-username/your-project.git` (for GitHub) or `git@gitlab.com:your-username/your-project.git` (for GitLab). This will be needed for the next step.

3. **Cloning the Project** 📥
   - Utilize the SSH URL noted in step 2. For instance, if the URL is `git@github.com:your-username/your-project.git`, run:
     ```
     git clone git@github.com:your-username/your-project.git
     ```

4. Successful cloning should be achieved, and you can access it with:
   ```
   cd your-project
   ```
🚀👨‍💻👩‍💻
