# 🧠 Quizzler-GUI-Quiz-App
<h2>🔎 Description:</h2>
<p>Quizzler is an interactive quiz game built using Python and Tkinter. It fetches true/false questions from the Open Trivia Database API and presents them to the user in a clean graphical interface. The player can answer each question by clicking True or False buttons, and the app gives immediate visual feedback (green for correct, red for incorrect) before loading the next question.</p>
<h3>🧱 Modules and Libraries Used:🧱 Modules and Libraries Used:</h3>
<ol>
  <li><strong>tkinter :</strong> To create the graphical user interface (GUI), including buttons, labels, canvas, and layout.</li>
  <li><strong>requests :</strong> To send an HTTP GET request to the trivia API and retrieve quiz data in JSON format.</li>
  <li><strong>html :</strong> To decode any HTML entities (like &quot; or &amp;) in the questions returned by the API.</li>
</ol><br>
<h3>💡 Project Structure:</h3>
<p>
quizzler/<br>
│<br>
├── main.py                # App runner and setup<br>
├── question_model.py      # Defines the Question class<br>
├── quiz_brain.py          # Core quiz logic<br>
├── ui.py                  # GUI layout and event handling<br>
├── images/<br>
│   ├── true.png<br>
│   └── false.png<br>
</p><br>
<h3>✅ API Used:</h3>
<p>Open Trivia DB (OpenTDB)</p>
<ul>
  <li><strong>URL:</strong> <a href="https://opentdb.com/api.php" target="_blank">https://opentdb.com/api.php</a></li>
  <il><strong>Purpose</strong> Provides trivia questions of various categories and types. This implementation uses <code>type=boolean</code> to fetch True/False questions.</il>
  <li><strong>Parameters Used:</strong>
    <ul>
      <li><strong>amount=30</strong> → Number of questions to fetch</li>
      <li><strong>type=boolean</strong> → Only true/false questions</li>
    </ul>
  </li><br>
  <li><strong>📥 Sample API Request</strong></li><br>
   <p> https://opentdb.com/api.php?amount=30&amp;type=boolean
  </p><br>
  <li><strong>📤 Sample API Response</strong></li><br>
  <p> {<br>
      "response_code": 0,<br>
      "results": [<br>
        {<br>
          "category": "Science: Computers",<br>
          "type": "boolean",<br>
          "difficulty": "easy",<br>
          "question": "Linus Torvalds created Linux and Git.",<br>
          "correct_answer": "True",<br>
          "incorrect_answers": ["False"]<br>
        },<br>
        ...<br>
      ]<br>
    }<br>
  </p><br>
  <li><strong>📚 Documentation</strong> <a href="https://opentdb.com/api_config.php" target="_blank">https://opentdb.com/api_config.php</a></li>
</ul>









