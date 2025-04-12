# Intro to Setting Up Your Penetration Testing Lab

When starting a penetration testing or cybersecurity course, a good lab environment is essential. Many courses—including the one I’m currently taking—recommend downloading a pre-built `.ova` file to import into VirtualBox for quick setup. However, I hit a roadblock that required a workaround, and I’ll walk you through it below.

## What is a Virtual Machine Lab Setup?

A virtual machine (VM) lab is a self-contained environment that allows you to safely practice offensive security techniques like vulnerability scanning, exploitation, and more—without putting your real system at risk. Tools like VirtualBox let you run these environments using files like `.ova` or `.vdi`.

## Real-World Use Case

Security professionals use virtual labs every day for testing exploits, verifying vulnerabilities, or demonstrating proof of concepts. Red teamers and bug bounty hunters often build small lab setups to simulate attacks on vulnerable targets before trying them out in the wild or in authorized programs.

---

## Lab Walkthrough

### 1. Target Environment

The course initially instructed us to download a `.ova` file and import it into VirtualBox as an appliance. Unfortunately, the provided link now redirects to the Kali Linux homepage (https://www.kali.org), and the `.ova` file is no longer directly available.

### Updated Process

Instead of importing an appliance (`.ova`), I had to manually download a VirtualBox image in `.vdi` format from Kali’s official site and create a new VM manually. Here’s how:

#### Step-by-Step: Create a VM Using a `.vdi` File

1. Go to [https://www.kali.org/get-kali/#kali-virtual-machines](https://www.kali.org/get-kali/#kali-virtual-machines)  
2. Download the VirtualBox version (`.vdi`) of Kali Linux  
3. Open VirtualBox and click **"New"**  
4. Set:
   - **Name:** Kali Linux  
   - **Type:** Linux  
   - **Version:** Debian (64-bit)  
5. Assign RAM (recommend at least 2GB)  
6. On **Hard disk**, choose **Use an existing virtual hard disk file**  
7. Browse to the `.vdi` file you downloaded and select it  
8. Finish the setup and start your VM  

### Screenshot

![Kali VM Setup Screenshot](./images/kali_vm_setup.png)

---

## Takeaways

- **Problem:** The course’s `.ova` file link is outdated and redirects to kali.org  
- **Solution:** Use the `.vdi` image instead and manually create a VM in VirtualBox  
- **Lesson:** Always double-check download links and be ready to adapt if course instructions are outdated  

---

## Screenshots

- [x] Screenshot of Kali VM setup in VirtualBox  
- [ ] Screenshot of successful boot/login  
- [ ] Screenshot of VirtualBox settings page  
