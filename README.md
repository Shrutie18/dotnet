KubernetesAPI  Dotnet build and deployment.
step 1) create an uubuntu instance.

![image](https://github.com/user-attachments/assets/2e8ddff6-7170-4f00-bab4-d9e22bc89ce6)
step 2) Ensure Snap is Installed

Snap should be pre-installed on Ubuntu 22.04, but you can verify and install it if needed.
step 3)sudo apt update
![image](https://github.com/user-attachments/assets/b16066b0-94a1-40e6-8685-04139b51cda2)

step4)Install Snap (if not already installed)
   
      sudo apt install snapd
      ![image](https://github.com/user-attachments/assets/73e1d8df-881d-4fa7-b4c8-6c9723803459)

      
  enable Snap  (if not already enabled):
   Make sure that Snap is enabled and running:
   
   sudo systemctl enable --now snapd.socket
   ![image](https://github.com/user-attachments/assets/d9b11908-4fa5-4afc-ae5b-f474366d189f)

step 2: Install .NET 6.0 SDK via Snap

1. **Install the .NET SDK** using the Snap command:
   
   sudo snap install dotnet-sdk --classic --channel=6.0
   ![image](https://github.com/user-attachments/assets/b21e25a8-a2c3-4209-a792-20e2d02eb370)

    Step 3: Create a Snap Alias for the `dotnet` Command

Snap packages often require fully qualified names, so you'll create an alias to use `dotnet` as a simpler command.

1. **Create the alias** for `dotnet`:
   
   sudo snap alias dotnet-sdk.dotnet dotnet
   
![image](https://github.com/user-attachments/assets/86cd47b0-7180-4a06-bf67-ce5e3819e80c)
Step 4: Verify the Installation

Once the installation and alias are set, verify that .NET 6.0 is properly installed:

1. **Check the .NET version**:

   dotnet --version
   ![image](https://github.com/user-attachments/assets/56aa0399-508d-4364-ae59-5cd1c351cbb0)
   
### Step 5: Create and Run a Sample .NET Application:

Deploying KubernetesCLusterAPI on dotnet.

1. Git clone project file and change directory to .cproj directory
   


   
