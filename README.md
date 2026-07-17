# CoFounder 🚀

**Your AI CoFounder: Turn raw ideas into an operational startup in seconds.**

* **Hackathon:** OpenAI Build Week
* **Codex Session ID:** `[MASUKKAN_SESSION_ID_ANDA_DI_SINI]`

---

## 🤖 How Codex & GPT-5.6 Were Used
To build a truly dynamic digital CoFounder, this project leverages OpenAI's models in two distinct and crucial pipelines:

* **GPT-5.6 Terra (The Strategist):** Used to process the entrepreneur's raw, unstructured business idea and transform it into highly structured business intelligence. It powers the "Business Work" and "Financial Calculator" by generating the comprehensive Lean Canvas, cost breakdowns, and strategic operational logic required to start the business.
* **OpenAI Codex (The Developer):** This is the core engine for our "Automated Systems" feature. We push the boundaries of Codex by not just asking for code snippets, but by commanding it to dynamically generate live, fully functional UI components (built in React and styled with Tailwind CSS) directly onto the entrepreneur's screen in real-time. It acts as an instant software developer for non-technical founders.

---

## Inspiration
Every year, many young people and single mothers, single fathers who have business ideas are forced to abandon their business ideas without having time to start them. They face several obstacles, namely:

* **Strategic Obstacles:** They do not know how to make a business plan, assess financial feasibility or prepare legal plans such as brand descriptions. This is because most of them lack basic knowledge about business and also access to information about business.
* **Technical Implementation Obstacles:** They also do not know how to record the basic business operating tools needed to launch. This is because they do not receive training from institutions responsible for business.

I created a Solution that acts as a **Business Consultant** and **AI Automation** by using OpenAI's GPT-5.6 and Codex APIs. I realized that this Solution can shorten the time from idea to reality.

## What it does
**CoFounder** is an all-in-one digital Co-founder for individual entrepreneurs. Entrepreneurs simply type in their raw, random ideas (e.g., *”Drive-thru Bakery”*), and the app instantly generates a structured draft of the startup ecosystem that can be divided into 3:

1. **Business Work:** I help entrepreneurs create a complete business plan using the Lean Canvas model. It includes a budget, a way to make money, and all the documents they need to register a business or trademark.
2. **Automated Systems:** Business system documents such as customer forms or inventory modules that are custom-built for businesses. All the code will be automatically generated and the app’s display will appear on the entrepreneur's screen immediately.
3. **Interactive Profit Calculator:** The app will automatically calculate the costs and revenues of the entrepreneur’s business. Entrepreneurs can adjust the price or sales volume using the ‘slider’ to see the profit graph change directly on the screen.

## How we built it
I design complete business applications from A to Z, with a simple and easy design that prioritizes speed and fluidity:
* **Simple Interface Design:** Built in **React** and styled with **Tailwind CSS**. I use a two-panel design. You type commands in the left panel, and see the results appear instantly in the right panel which has three navigation tabs for quick access.
* **Behind-the-Scenes Technology:** Using **FastAPI** (Python) which acts as a link between the user and the AI ​​(OpenAI), ensuring that all processes run smoothly.
* **Automated Planning & Development:** My AI not only plans business strategies for entrepreneurs, but also 'writes' the entrepreneurs' application code directly. All generated code is securely sent to the entrepreneurs' screens and displayed in the form of a fully functional application.

## Challenges we ran into
* **Innovation in Stability:** The biggest challenge was safely integrating the 'raw' code from the AI ​​into existing applications. By developing an isolated and secure code processing pipeline, I was able to ensure that the entrepreneur's application was always stable and ready to use without any technical glitches.
* **Financial Data Accuracy:** For the profit calculator to work properly, the AI ​​needed to convert the entrepreneur's simple ideas into precise numbers. I built a data reconciliation system that ensured that every input from the entrepreneur was translated into consistent and accurate economic calculations every time the entrepreneur used it.

## Accomplishments that we're proud of
* **Instant Business in a Minute:** I managed to get to the point where entrepreneurs only need to describe their business idea in one paragraph, and the system continues to build complete forms and functions for the entrepreneur in minutes.
* **A Very Smooth System:** The combination of modern technologies allows the application to move very quickly. Charts and information change instantly before the entrepreneur's eyes without having to reload the page—providing a very comfortable and responsive entrepreneur experience.

## What we learned
I found that the combination of GPT-5.6 and Codex has changed the way we work: instead of just “reading text”, we can now directly “build systems that work”. I learned that AI is very helpful in building complex user interfaces (UI) as long as we give it the right instructions. In addition, properly structuring work steps is the key to building fast and stable web applications. For example, we tested AI’s ability to build a financial calculator.

Using the basic formula of return on capital:

$$V_d = \frac{C_f}{30 \times (P_u - C_v)}$$

(Where $V_d$ is the daily sales required, $C_f$ is the monthly fixed cost, while $P_u$ and $C_v$ are the price and cost per unit of the product, respectively).

Seeing AI translate this formula into a ready-to-use interactive calculator in an instant really proves that the future of business is using “AI Agents” that can do the work automatically for entrepreneurs.

## What's next for CoFounder
* **Save & Continue Entrepreneur Work:** I am building functionality so that Entrepreneurs can save their work, download application code directly to GitHub, and manage multiple business ideas in one place.
* **Smart Agent Team:** I will introduce specialized "expert agents". For example, there will be a Marketing Agent (CMO) for sales strategy, and a Finance Agent (CFO) for more in-depth and thorough budget simulations.
* **Real Sales Testing:** I will enable AI to build a payment system (Stripe) in the entrepreneur's app. With this, entrepreneurs can start testing whether customers really want to buy their products from day one.

---

## 💻 Setup Instructions (How to Run Locally)

To run **IdeaNation CoFounder** on your local machine, you will need to start both the Python backend and the React frontend.

### Prerequisites
* Python 3.9+
* Node.js and npm
* OpenAI API Key (with access to GPT-5.6 and Codex)

### 1. Backend Setup (FastAPI)
Open a terminal and navigate to the project root, then into the backend folder:
```bash
cd backend
# Create and activate virtual environment
python -m venv venv
# On Windows: venv\Scripts\activate
# On Mac/Linux: source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Set your API Key
export OPENAI_API_KEY="your-api-key-here"

# Run the backend server
uvicorn main:app --reload
