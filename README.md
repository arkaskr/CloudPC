# CloudPC
Easily set up a free Windows Server VPS using GitHub and Ngrok, and access it from anywhere in the world via Windows Remote Desktop (RDP). Follow the step-by-step instructions to create a powerful remote server without any cost.


### README:

# Free Windows Server VPS with GitHub and Ngrok

This repository provides a step-by-step guide to create a free Windows Server VPS using GitHub Actions and Ngrok. You will be able to access your server from anywhere using Windows Remote Desktop (RDP).

## Features
- **Free Windows Server VPS**: Set up a free Windows Server instance.
- **Global Access**: Use Ngrok to access your server from anywhere in the world.
- **Easy RDP Access**: Connect to your server via Windows Remote Desktop.

## Requirements
- A GitHub account
- Ngrok account (Free tier works)
- Basic knowledge of GitHub and RDP

## Setup Instructions

### 1. Fork the Repository
Fork this repository to your own GitHub account.

### 2. Generate Ngrok Authentication Token
1. Sign up for an Ngrok account at [Ngrok](https://ngrok.com/).
2. After signing in, go to the [Auth section](https://dashboard.ngrok.com/get-started/your-authtoken) to get your authentication token.

### 3. Add Ngrok Token to GitHub Secrets
1. Go to your forked repository on GitHub.
2. Navigate to `Settings` > `Secrets and variables` > `Actions`.
3. Click on `New repository secret`.
4. Add a new secret with the name `NGROK_AUTH_TOKEN` and paste your Ngrok authentication token as the value.

### 4. Enable GitHub Actions
1. Go to the `Actions` tab in your forked repository.
2. Click on the `Windows Server Setup` workflow.
3. Enable the workflow by clicking on `Run workflow`.

### 5. Start the GitHub Action
1. Trigger the workflow manually by going to the `Actions` tab and selecting `Run workflow` under `Windows Server Setup`.

### 6. Retrieve RDP Credentials and Ngrok URL
1. Once the workflow is complete, go to the `Actions` tab.
2. Select the latest workflow run and click on it.
3. In the workflow details, you will find the RDP credentials and the Ngrok URL to connect to your Windows Server.

### 7. Connect via Windows Remote Desktop (RDP)
1. Open the Remote Desktop Connection application on your computer.
2. Enter the Ngrok URL provided in the workflow details.
3. Use the RDP credentials to log in.

## Troubleshooting
- Ensure your Ngrok token is correct.
- Make sure the GitHub Actions workflow has completed successfully.
- Check Ngrok status on the dashboard if you have connection issues.

## Contributing
Feel free to submit issues or pull requests if you have suggestions for improvements or find any bugs.

## License
This project is licensed under the MIT License.

---

By following these steps, you can have a free, globally accessible Windows Server VPS up and running in no time. Enjoy your new server!
