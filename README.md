# Episode-48: Claude Code Remote-Control Server

Running Claude Code as a remote-control server

## Running Claude Code as a Remote-Control Server 

Carl and Rocky show how you can set up Claude Code on your workstation so you can create and connect to multiple sessions remotely from your phone or Claude Desktop.

📺 YouTube video: 

🏠 Code it with AI Home Page: [https://codeitwithai.com](https://codeitwithai.com/)

## Blog posts

* [Remote access to Claude Code or GitHub Copilot via SSH](https://blog.lhotka.net/2026/09/18/SSH-Is-Not-A-Desktop)
* [Set up Claude Code as a remote-control server](https://blog.lhotka.net/2026/09/21/Remote-Control-Server)

## Discussion

I (Rocky) travel a lot, and want to use my AI coding tools from the airplane, hotels, or other locations where bandwidth might be limited.

Using Claude Code or GitHub Copilot _locally_ consumes a lot of bandwidth and is often unusable.

I tried using SSH (secure shell) to connect to my workstation, but if SSH loses connection then your work is lost.

I tried using normal remote-control from Claude Code and GitHub Copilot, which is quite good. But if your workstation reboots (Patch Tuesday anyone?) you lose access to your remote sessions.

Fortunately, it turns out that you can run Claude Code as a Windows service (or daemon on Linux) and it will host up to 32 remote sessions that survive a workstation reboot!

From your phone, it looks like this when you create a new code session:

<img width="1079" height="1132" alt="Screenshot_20260925-000537" src="https://github.com/user-attachments/assets/2593d48c-f1be-494b-9559-8f7a3ed62ca3" />

Once you have some sessions running, your code window looks something like this:

<img width="1080" height="2201" alt="Screenshot_20260925-092112" src="https://github.com/user-attachments/assets/dcdd0e7d-a7f2-4d22-99a2-d0b5c6c34db8" />

There is a similar (though not as polished) experience from Claude Desktop.
