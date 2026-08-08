
■ BOOT PROCESS (Remember: BIOS → GRUB → Kernel → systemd → Login)
motherboard lights up and CPU executes BIOS ( since cpu is connected on motherboard and motherboard act as powersupply to cpu)
motherboard has power-delivery circuitry (VRMs) that converts/regulates the PSU's power into the voltages the CPU needs.
1. BIOS/UEFI → (BIOS is stored on the motherboard) Hardware check (POST power on self test) also detect devices  .
2. Bootloader (GRUB) → Select OS, finds load kernel.
3. Kernel → memory, drivers, mount root filesystem.
4. systemd (PID 1) → Start services and targets.
5. Login → tty or GUI


SHELL = User talks to Kernel
Flow: User → Shell → Kernel → Hardware
Must remember:
• pwd = where am I
• ls = show files
• cd = change folder
• cp / mv / rm = copy move delete
• cat = view file
• grep = search text
• chmod = permissions
• sudo = run as root



■■ systemd (PID 1) — Service Manager
 when i do command like systemctl status sshd i mean
 You → systemd

“Hey systemd, what is happening with the sshd service?”
