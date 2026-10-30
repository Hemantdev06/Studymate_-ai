# index.html



<!DOCTYPE html>

<html lang="en">

<head>

<meta charset="UTF-8">

<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>StudyMate AI</title>



<style>

\* {

&#x20;   margin: 0;

&#x20;   padding: 0;

&#x20;   box-sizing: border-box;

}



body {

&#x20;   font-family: Arial, sans-serif;

&#x20;   background: #f3f4fc;

&#x20;   color: #252344;

}



/\* Header \*/



header {

&#x20;   background: linear-gradient(120deg, #34218e, #7356df);

&#x20;   color: white;

&#x20;   padding: 22px 6%;

}



.logo {

&#x20;   font-size: 25px;

&#x20;   font-weight: bold;

}



.logo span {

&#x20;   color: #b9adff;

}



header p {

&#x20;   margin-top: 7px;

&#x20;   color: #e2dcff;

}



/\* Main layout \*/



.layout {

&#x20;   display: flex;

&#x20;   max-width: 1250px;

&#x20;   margin: 30px auto;

&#x20;   gap: 22px;

&#x20;   padding: 0 20px;

}



/\* Sidebar \*/



.sidebar {

&#x20;   width: 230px;

&#x20;   background: white;

&#x20;   padding: 22px;

&#x20;   border-radius: 15px;

&#x20;   height: fit-content;

&#x20;   box-shadow: 0 5px 20px #2221;

}



.sidebar h3 {

&#x20;   margin-bottom: 20px;

&#x20;   color: #6b50d8;

}



.nav-item {

&#x20;   padding: 13px;

&#x20;   margin-bottom: 10px;

&#x20;   border-radius: 9px;

&#x20;   background: #f2efff;

&#x20;   cursor: pointer;

&#x20;   font-size: 14px;

}



.nav-item:hover {

&#x20;   background: #ddd5ff;

}



/\* Main content \*/



.main {

&#x20;   flex: 1;

&#x20;   min-width: 0;

}



.welcome {

&#x20;   margin-bottom: 22px;

}



.welcome h2 {

&#x20;   font-size: 26px;

&#x20;   margin-bottom: 8px;

}



.welcome p {

&#x20;   color: #77748b;

}



/\* Feature cards \*/



.features {

&#x20;   display: grid;

&#x20;   grid-template-columns: repeat(3, 1fr);

&#x20;   gap: 13px;

&#x20;   margin-bottom: 23px;

}



.feature {

&#x20;   background: white;

&#x20;   padding: 18px 12px;

&#x20;   border-radius: 13px;

&#x20;   text-align: center;

&#x20;   box-shadow: 0 3px 15px #2221;

}



.feature .emoji {

&#x20;   font-size: 27px;

&#x20;   margin-bottom: 9px;

}



.feature h4 {

&#x20;   color: #4732b0;

&#x20;   font-size: 14px;

}



.feature p {

&#x20;   font-size: 11px;

&#x20;   color: #888;

&#x20;   margin-top: 6px;

}



/\* Editor \*/



.editor {

&#x20;   background: white;

&#x20;   padding: 24px;

&#x20;   border-radius: 15px;

&#x20;   box-shadow: 0 4px 18px #2221;

}



.editor h3 {

&#x20;   margin-bottom: 10px;

}



textarea {

&#x20;   width: 100%;

&#x20;   height: 190px;

&#x20;   border: 1px solid #dedbec;

&#x20;   border-radius: 10px;

&#x20;   padding: 15px;

&#x20;   font-size: 15px;

&#x20;   resize: vertical;

&#x20;   outline: none;

&#x20;   margin: 14px 0;

&#x20;   font-family: Arial;

}



textarea:focus {

&#x20;   border-color: #7356df;

}



label {

&#x20;   display: block;

&#x20;   margin: 10px 0;

&#x20;   font-weight: bold;

&#x20;   font-size: 14px;

}



select {

&#x20;   width: 100%;

&#x20;   padding: 12px;

&#x20;   border: 1px solid #ddd;

&#x20;   border-radius: 8px;

&#x20;   margin-bottom: 15px;

&#x20;   background: white;

}



.actions {

&#x20;   display: flex;

&#x20;   flex-wrap: wrap;

&#x20;   gap: 10px;

}



button {

&#x20;   border: none;

&#x20;   padding: 12px 17px;

&#x20;   border-radius: 8px;

&#x20;   cursor: pointer;

&#x20;   font-size: 14px;

&#x20;   font-weight: bold;

}



.primary {

&#x20;   background: linear-gradient(120deg, #5035c8, #8768ec);

&#x20;   color: white;

}



.secondary {

&#x20;   background: #eeeaff;

&#x20;   color: #4932ad;

}



button:hover {

&#x20;   opacity: 0.85;

}



button:disabled {

&#x20;   opacity: 0.5;

&#x20;   cursor: wait;

}



/\* Results \*/



.result {

&#x20;   margin-top: 22px;

&#x20;   padding: 22px;

&#x20;   background: white;

&#x20;   border-radius: 15px;

&#x20;   box-shadow: 0 4px 18px #2221;

}



.result h3 {

&#x20;   color: #4932ad;

&#x20;   margin-bottom: 14px;

}



\#output {

&#x20;   white-space: pre-wrap;

&#x20;   line-height: 1.8;

&#x20;   color: #444;

&#x20;   min-height: 60px;

}



.result-buttons {

&#x20;   margin-top: 15px;

&#x20;   display: flex;

&#x20;   gap: 10px;

&#x20;   flex-wrap: wrap;

}



footer {

&#x20;   text-align: center;

&#x20;   padding: 25px;

&#x20;   color: #888;

&#x20;   font-size: 13px;

}



@media(max-width: 750px) {

&#x20;   .layout {

&#x20;       flex-direction: column;

&#x20;   }



&#x20;   .sidebar {

&#x20;       width: 100%;

&#x20;   }



&#x20;   .features {

&#x20;       grid-template-columns: 1fr;

&#x20;   }



&#x20;   .welcome h2 {

&#x20;       font-size: 22px;

&#x20;   }

}

</style>

</head>



<body>



<header>

&#x20;   <div class="logo">📚 StudyMate <span>AI</span></div>

&#x20;   <p>Your smart AI-powered study assistant</p>

</header>



<div class="layout">



&#x20;   <aside class="sidebar">

&#x20;       <h3>Navigation</h3>



&#x20;       <div class="nav-item" onclick="clearAll()">

&#x20;           🏠 Dashboard

&#x20;       </div>



&#x20;       <div class="nav-item" onclick="setMode('summary')">

&#x20;           📝 AI Summary

&#x20;       </div>



&#x20;       <div class="nav-item" onclick="setMode('keypoints')">

&#x20;           ⭐ Key Points

&#x20;       </div>



&#x20;       <div class="nav-item" onclick="setMode('mcq')">

&#x20;           ❓ MCQ Generator

&#x20;       </div>

&#x20;   </aside>



&#x20;   <main class="main">



&#x20;       <div class="welcome">

&#x20;           <h2>Welcome to StudyMate AI 👋</h2>

&#x20;           <p>Make your study preparation smarter and easier.</p>

&#x20;       </div>



&#x20;       <div class="features">



&#x20;           <div class="feature">

&#x20;               <div class="emoji">📝</div>

&#x20;               <h4>Smart Summary</h4>

&#x20;               <p>Shorten lengthy notes</p>

&#x20;           </div>



&#x20;           <div class="feature">

&#x20;               <div class="emoji">⭐</div>

&#x20;               <h4>Key Points</h4>

&#x20;               <p>Find important topics</p>

&#x20;           </div>



&#x20;           <div class="feature">

&#x20;               <div class="emoji">❓</div>

&#x20;               <h4>MCQ Generator</h4>

&#x20;               <p>Practice questions</p>

&#x20;           </div>



&#x20;       </div>



&#x20;       <section class="editor">



&#x20;           <h3>📖 Enter Your Study Notes</h3>



&#x20;           <p style="color:#888;font-size:14px;">

&#x20;               Paste your chapter or study material below.

&#x20;           </p>



&#x20;           <textarea id="notes"

&#x20;           placeholder="Paste your notes here..."></textarea>



&#x20;           <label>Summary Length</label>



&#x20;           <select id="length">

&#x20;               <option value="short">Short</option>

&#x20;               <option value="medium" selected>Medium</option>

&#x20;               <option value="detailed">Detailed</option>

&#x20;           </select>



&#x20;           <label>Choose Your Feature</label>



&#x20;           <select id="mode">

&#x20;               <option value="summary">AI Summary</option>

&#x20;               <option value="keypoints">Important Key Points</option>

&#x20;               <option value="mcq">Generate MCQs</option>

&#x20;           </select>



&#x20;           <div class="actions">

&#x20;               <button class="primary" id="generate"

&#x20;               onclick="generateResult()">

&#x20;                   ✨ Generate Result

&#x20;               </button>



&#x20;               <button class="secondary"

&#x20;               onclick="clearAll()">

&#x20;                   Clear Notes

&#x20;               </button>

&#x20;           </div>



&#x20;       </section>



&#x20;       <section class="result">



&#x20;           <h3>✨ Generated Results</h3>



&#x20;           <div id="output">

&#x20;               Your generated result will appear here.

&#x20;           </div>



&#x20;           <div class="result-buttons">

&#x20;               <button class="secondary"

&#x20;               onclick="copyResult()">

&#x20;                   📋 Copy

&#x20;               </button>



&#x20;               <button class="secondary"

&#x20;               onclick="downloadResult()">

&#x20;                   ⬇ Download

&#x20;               </button>

&#x20;           </div>



&#x20;       </section>



&#x20;   </main>



</div>



<footer>

&#x20;   Made with ❤️ by StudyMate AI | Smart Learning for Everyone

</footer>



<script>



function setMode(mode) {

&#x20;   document.getElementById("mode").value = mode;

&#x20;   document.querySelector(".editor").scrollIntoView({

&#x20;       behavior: "smooth"

&#x20;   });

}



function clearAll() {

&#x20;   document.getElementById("notes").value = "";

&#x20;   document.getElementById("output").textContent =

&#x20;       "Your generated result will appear here.";

}



function generateResult() {



&#x20;   let text = document.getElementById("notes").value.trim();

&#x20;   let mode = document.getElementById("mode").value;

&#x20;   let length = document.getElementById("length").value;



&#x20;   if (!text) {

&#x20;       alert("Please enter your study notes!");

&#x20;       return;

&#x20;   }



&#x20;   if (text.length < 30) {

&#x20;       alert("Please enter at least 30 characters!");

&#x20;       return;

&#x20;   }



&#x20;   let output = "";



&#x20;   if (mode === "summary") {



&#x20;       let sentences = text.match(/\[^.!?]+\[.!?]+|\[^.!?]+$/g) || \[];



&#x20;       let count = length === "short" ? 2 :

&#x20;                   length === "medium" ? 4 : sentences.length;



&#x20;       output = "📝 AI SUMMARY\\n\\n" +

&#x20;       sentences.slice(0, count).join(" ").trim();



&#x20;   }



&#x20;   else if (mode === "keypoints") {



&#x20;       let points = text.split(/\[.!?]+/)

&#x20;       .map(s => s.trim())

&#x20;       .filter(s => s.length > 10);



&#x20;       output = "⭐ IMPORTANT KEY POINTS\\n\\n";



&#x20;       points.forEach((point, index) => {

&#x20;           output += (index + 1) + ". " + point + "\\n\\n";

&#x20;       });



&#x20;   }



&#x20;   else if (mode === "mcq") {



&#x20;       let words = text.match(/\\b\[A-Za-z]{5,}\\b/g) || \[];

&#x20;       words = \[...new Set(words)];



&#x20;       if (words.length < 4) {

&#x20;           alert("Please enter more detailed notes!");

&#x20;           return;

&#x20;       }



&#x20;       output = "❓ PRACTICE MCQs\\n\\n";



&#x20;       words.slice(0, 5).forEach((word, index) => {



&#x20;           output += (index + 1) + ". Which word appears in your notes?\\n";

&#x20;           output += "A. " + word + "\\n";

&#x20;           output += "B. Apple\\n";

&#x20;           output += "C. School\\n";

&#x20;           output += "D. Computer\\n";

&#x20;           output += "Answer: " + word + "\\n\\n";



&#x20;       });



&#x20;   }



&#x20;   document.getElementById("output").textContent = output;



}



function copyResult() {



&#x20;   let text = document.getElementById("output").innerText;



&#x20;   if (!text || text === "Your generated result will appear here.") {

&#x20;       alert("Generate a result first!");

&#x20;       return;

&#x20;   }



&#x20;   navigator.clipboard.writeText(text)

&#x20;   .then(() => alert("Result copied!"))

&#x20;   .catch(() => alert("Please select and copy the result manually."));



}



function downloadResult() {



&#x20;   let text = document.getElementById("output").innerText;



&#x20;   if (!text || text === "Your generated result will appear here.") {

&#x20;       alert("Generate a result first!");

&#x20;       return;

&#x20;   }



&#x20;   let file = new Blob(\[text], {type: "text/plain"});

&#x20;   let link = document.createElement("a");



&#x20;   link.href = URL.createObjectURL(file);

&#x20;   link.download = "StudyMate-Notes.txt";

&#x20;   link.click();



&#x20;   URL.revokeObjectURL(link.href);



}



</script>



</body>

</html>





# script.js



let studyMateEngine = null;

let studyMateLoading = null;



// Load the AI model in the browser

async function loadStudyMateAI() {

&#x20;   if (!navigator.gpu) {

&#x20;       throw new Error(

&#x20;           "WebGPU is not available. Try updated Chrome or Edge."

&#x20;       );

&#x20;   }



&#x20;   if (!studyMateLoading) {

&#x20;       studyMateLoading = (async () => {



&#x20;           const webllm = await import(

&#x20;               "https://esm.run/@mlc-ai/web-llm"

&#x20;           );



&#x20;           const model =

&#x20;               "Qwen2-0.5B-Instruct-q4f16\_1-MLC";



&#x20;           studyMateEngine =

&#x20;               await webllm.CreateMLCEngine(

&#x20;                   model,

&#x20;                   {

&#x20;                       initProgressCallback: (progress) => {

&#x20;                           const loading =

&#x20;                               document.getElementById("loading");



&#x20;                           if (loading) {

&#x20;                               loading.textContent =

&#x20;                                   progress.text;

&#x20;                           }

&#x20;                       }

&#x20;                   }

&#x20;               );



&#x20;           return studyMateEngine;

&#x20;       })();

&#x20;   }



&#x20;   return studyMateLoading;

}



// Send a prompt to the local AI

async function askStudyMateAI(prompt) {



&#x20;   const engine = await loadStudyMateAI();



&#x20;   const response =

&#x20;       await engine.chat.completions.create({

&#x20;           messages: \[

&#x20;               {

&#x20;                   role: "system",

&#x20;                   content:

&#x20;                       "You are StudyMate AI, a helpful study assistant. Give accurate, clear and student-friendly answers."

&#x20;               },

&#x20;               {

&#x20;                   role: "user",

&#x20;                   content: prompt

&#x20;               }

&#x20;           ],

&#x20;           temperature: 0.7,

&#x20;           max\_tokens: 700

&#x20;       });



&#x20;   return response.choices\[0].message.content;

}

