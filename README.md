<h1 align="center">Kalpan - Full Stack Developer Terminal</h1>

<div align="center">
   <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&duration=2000&pause=1000&color=16F7C6&center=true&vCenter=true&width=500&height=45&lines=Welcome+to+Kalpan's+Terminal...;Type+%22skills%22+to+see+tech+stack...;Type+%22projects%22+to+view+my+work...">
</div>

<!-- Terminal Design -->
<div align="center">
   <pre style="background-color:black;color:green;padding:20px;border-radius:10px;width:80%;text-align:left;">
   <span id="terminal-output"></span>
   <br>
   <span style="color:lightblue;">$</span> <span id="terminal-input">|</span>
   </pre>
</div>

<script>
   const commands = [
      { cmd: "skills", response: "HTML5, CSS3, JavaScript, React, Node.js, MongoDB, C, C++" },
      { cmd: "projects", response: "1. React API Project\n2. YouTube Clone (yt-react)\n3. Pass-Gen-React (Password Generator)" },
      { cmd: "contact", response: "Email: kalpankaneriya@gmail.com\nLinkedIn: Kalpan2007" },
      { cmd: "clear", response: "" },
      { cmd: "about", response: "I'm Kalpan, a Full-Stack Developer learning and growing in web technologies." }
   ];

   let terminalOutput = document.getElementById("terminal-output");
   let terminalInput = document.getElementById("terminal-input");
   let index = 0;

   function typeText(text, delay) {
      let i = 0;
      terminalInput.textContent = "";
      let interval = setInterval(() => {
         terminalInput.textContent += text[i];
         i++;
         if (i === text.length) clearInterval(interval);
      }, delay);
   }

   function simulateTerminal() {
      let interval = setInterval(() => {
         if (index >= commands.length) index = 0;
         let { cmd, response } = commands[index];
         terminalOutput.innerHTML += `<br><span style='color:lightblue;'>$ ${cmd}</span><br>${response}`;
         index++;
      }, 5000);  // Changes every 5 seconds
   }

   simulateTerminal();
</script>

<h2 align="center">🔗 Connect with Me:</h2>
<p align="center">
   <a href="mailto:kalpankaneriya@gmail.com">
      <img align="center" src="https://cdn.worldvectorlogo.com/logos/official-gmail-icon-2020-.svg" alt="mail" height="50" width="55" />
   </a>
   &nbsp;&nbsp;&nbsp;
   <a href="https://linkedin.com/in/Kalpan2007">
      <img align="center" src="https://cdn.worldvectorlogo.com/logos/linkedin-icon-3.svg" alt="linkedin" height="50" width="50" />
   </a>
</p>
