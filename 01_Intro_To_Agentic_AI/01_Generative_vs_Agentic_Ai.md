# Lecture 1 — Generative AI vs Agentic AI

## 1. Start with one real question

Imagine you are an HR recruiter. Your company wants to hire a **remote Backend Engineer with 2–4 years of experience**.

Hiring ke liye tumhe sirf ek job description likhni nahi hai. You need to:

- Write the job description (JD).
- Publish it on job portals.
- Review resumes and shortlist suitable candidates.
- Schedule interviews and prepare interview questions.
- Send the offer letter to the selected candidate.
- Help with onboarding after the candidate joins.

Now imagine you have an AI chatbot. It can write the JD, draft emails, and prepare interview questions.

**But here's the question: if AI can do these individual tasks, can it manage the entire hiring process by itself?**

Not necessarily. Content generate karna aur ek complete goal ko end-to-end manage karna do different things hain. Isi difference ko samajhne ke liye pehle Generative AI se start karte hain.

## 2. What is Generative AI?

**Generative AI is AI that can create new content by learning patterns from data.**

Content different forms mein ho sakta hai. In forms ko **modalities** kehte hain.

- **Text:** ChatGPT jaise tools emails, explanations, summaries aur articles generate kar sakte hain.
- **Images:** Image-generation models written prompt se images bana sakte hain.
- **Code:** AI code likhne, explain karne aur debugging mein help kar sakti hai.
- **Audio:** Text-to-speech (TTS) tools written text ko spoken audio mein convert karte hain.
- **Video:** Video-generation models text description ke basis par video clips create kar sakte hain.

For example, tum prompt dete ho:

> Write a professional email inviting a candidate for a Backend Engineer interview.

AI email ka draft generate kar deti hai. Tumhe blank page se start nahi karna padta; you can review the draft, make changes, and use it.

**Yahi Generative AI ka core kaam hai: content create karna.**

### Where is Generative AI used?

- **Creative and business writing:** emails, blogs, reports and summaries.
- **Software development:** code suggestions, explanations and debugging help.
- **Customer support:** common customer questions ke answers.
- **Education:** difficult topics ko simple language mein explain karna.
- **Design and media:** images, designs, audio aur video content generate karna.

GenAI kaafi useful hai, but ab ek important distinction samjho: **a good answer is not the same as a completed real-world task.** Hiring example mein email draft kar dena useful hai, lekin candidate ko email send karna ek separate action hai.

## 3. Traditional AI vs Generative AI

Generative AI ko aur clearly samajhne ke liye, let's compare it with traditional AI—especially common supervised Machine Learning tasks.

### Traditional AI: predict or classify

A supervised ML model training examples se input aur expected output ke beech patterns learn karta hai. Phir new input milne par prediction karta hai.

Examples:

- Email → **spam** or **not spam**.
- Image → predicted category.
- Historical data → predicted value or outcome.

Simple words mein, model ka main kaam hota hai **input ke basis par output predict karna**.

### Generative AI: create new content

Generative AI learned patterns use karke new content generate karti hai.

- Traditional ML model email ko spam ya not spam classify kar sakta hai.
- Generative AI model email ka reply draft kar sakta hai.

So, common traditional ML examples prediction par focus karte hain, while Generative AI content creation par focus karti hai. Ye simplified comparison hai; har AI system ko strictly in do boxes mein divide nahi kiya ja sakta.

**Ab is idea ko hiring example par apply karte hain.** A chatbot can generate a JD, but kya woh company ke rules ko jaanta hai? Let's improve the chatbot step by step.

## 4. Stage One — Basic LLM chatbot

Suppose tum normal LLM-based chatbot use kar rahe ho. You can ask it to:

- Draft a Backend Engineer JD.
- Suggest suitable job portals.
- Explain what to look for in resumes.
- Prepare interview questions and invitation emails.
- Draft an offer letter.

Ye kaafi help karta hai. Writing ka time bachta hai, aur tumhe har document zero se create nahi karna padta.

### But what is missing?

- **It is mostly reactive:** tum prompt dete ho, tab chatbot answer deta hai. Next step ke liye usually tumhe phir prompt dena padta hai.
- **It doesn't automatically manage the full process:** JD draft hone ke baad publishing, screening aur interviews ki coordination tumhe karni padti hai.
- **It may lack company-specific knowledge:** general chatbot ko tumhari company's salary bands, screening rules, hiring policy ya preferred portals ka pata zaroori nahi hai.
- **Drafting isn't doing:** email draft kar dena aur email actually send karna same thing nahi hai.

Matlab chatbot individual tasks mein help kar raha hai, but **process ka coordinator abhi bhi tum ho**.

So, next question: *what if the chatbot could use our company's own hiring documents?*

## 5. Stage Two — RAG-based chatbot

Company ke paas already useful hiring information ho sakti hai:

- Previous job descriptions and successful-hire examples.
- Junior/senior aur remote/on-site role guidelines.
- Hiring playbook and preferred job portals.
- Salary bands and screening criteria.
- Interview question bank.
- Offer letter, welcome email and onboarding templates.

Agar chatbot ko in documents se relevant information retrieve karne aur answer banate waqt use karne ki ability di jaaye, toh this approach is called **Retrieval-Augmented Generation (RAG)**.

### How does it help?

1. You ask a question.
2. System company documents mein relevant information search karta hai.
3. The model uses that information to generate its answer.

For example, instead of asking only “Write a Backend Engineer JD,” tum keh sakte ho:

> Write a JD for a remote Backend Engineer with 2–4 years of experience, following our company's hiring guidelines.

Ab chatbot relevant company documents use karke more specific JD bana sakta hai. Answer generic advice ke bajay company ke process, criteria aur style ke closer hoga.

**RAG ka benefit: better context and more relevant answers.**

### But did we solve the whole problem?

Not yet.

- Chatbot ko pata ho sakta hai ki company ka preferred job portal kaunsa hai.
- But knowing the portal doesn't mean it can publish the JD there.
- It may know the correct email template, but that doesn't mean it can send the email.

**RAG knowledge access improve karta hai; by itself, it does not perform external actions.**

Toh next step kya hoga? Chatbot ko actual systems ke saath interact karne ki ability dena.

## 6. Stage Three — Tool-augmented chatbot

Now imagine chatbot ko external **tools or APIs** se connect kar diya gaya hai. Ye tools use karke woh other applications mein actions perform kar sakta hai.

Hiring example mein:

- **Job portal API:** vacancy publish ya update karne ke liye.
- **Resume parser:** resumes se relevant information extract karne ke liye.
- **Calendar API:** interview availability check aur schedule karne ke liye.
- **Email API:** candidate ko email send karne ke liye.
- **HR system:** hiring aur onboarding information manage karne ke liye.

Ab chatbot sirf JD draft nahi karega. With the right tool and permission, it may publish the approved JD, help process resumes, schedule interviews, or send emails.

### Follow the hiring process

- Job publish hoti hai.
- System application count check karta hai.
- Agar applications bahut kam hain, it can help identify the issue and suggest improving the JD or changing the promotion strategy.
- Relevant tools ke through, approved changes apply kiye ja sakte hain.
- Applications aane par system resumes compare karne, shortlist prepare karne aur interviews schedule karne mein help kar sakta hai.

This is a major improvement: the system now has access to relevant knowledge **and** the ability to take actions.

### One problem still remains

Tools available hain, but who decides what should happen next?

- Who notices that applications are too low?
- Who tracks which hiring steps are complete?
- Who decides whether the strategy should change?
- Who coordinates the entire process towards the final goal?

Agar recruiter ko har stage check karke chatbot ko next instruction deni pade, toh recruiter still manages the process.

**Tools make actions possible, but tools alone don't guarantee planning, progress tracking, or adaptation.**

And this brings us to Agentic AI.

## 7. Stage Four — Agentic AI

Ab imagine karo tum chatbot ko har small task separately dene ke bajay ek overall goal dete ho:

> Help me hire a remote Backend Engineer with 2–4 years of experience.

An **Agentic AI system** can coordinate multiple steps towards that goal. It can make a plan, use available tools, track progress, observe results, and choose a suitable next step based on what is happening.

### Let's see how it behaves

- **Plan the work:** system identifies that hiring involves a JD, job publishing, applications, screening, interviews, an offer, and onboarding.
- **Start with the first steps:** it drafts the JD and can ask for approval before publishing it.
- **Track progress:** after publishing, it checks application progress if it has the required access.
- **Notice problems:** if very few suitable applications arrive, it can flag the issue instead of continuing blindly.
- **Suggest an adjustment:** it may recommend improving the JD or changing the promotion strategy.
- **Use tools after approval:** with the right permissions, it can apply approved changes and continue coordinating the process.
- **Move to the next stage:** as applications arrive, it can help screen resumes, schedule interviews, prepare interview material, and support offer/onboarding steps.

Notice the difference? The system is not simply waiting for a new prompt for every small task. It is working towards the larger hiring goal and using the results of earlier steps to decide what makes sense next.

### Three ideas to understand this behaviour

**1. Proactive behaviour**

A basic chatbot usually waits for your next prompt. An agentic system, if designed with the right access and monitoring, can notice that applications are low and bring the issue to your attention.

**2. Progress and context**

The system needs to know what has already happened and what is still pending. Agar JD publish ho chuki hai, it should treat that step as completed—not start from the beginning every time.

**3. Adaptability**

Real-world tasks don't always go exactly as planned. If the first hiring strategy does not bring enough applications, the system should be able to identify the problem and consider a different next step.

These ideas are connected: **the system tracks the goal, observes what happens, and adapts its next action based on the result.**

### Does Agentic AI mean no human involvement?

No. Human approval can still be essential.

- The system may draft and recommend actions.
- A recruiter can review the JD before publishing.
- Important decisions, such as final candidate selection or sending an offer, can require approval.
- The system's autonomy depends on how it is designed and what permissions it has.

Goal coordination doesn't mean giving AI unlimited authority. It means letting it handle appropriate steps while keeping humans involved where judgement and approval matter.

## 8. Connect all four stages

The hiring example shows how each stage solves a different limitation.

**Basic LLM chatbot**
- Generates useful content.
- But human still guides each step.

**RAG-based chatbot**
- Uses relevant company documents.
- Answers become more company-specific.
- But RAG alone doesn't perform external actions.

**Tool-augmented chatbot**
- Can interact with job portals, calendars, email and HR systems.
- But tool access alone doesn't guarantee goal planning or progress tracking.

**Agentic AI system**
- Coordinates multiple steps around the hiring goal.
- Tracks progress and observes results.
- Uses tools and adapts the next step when needed.
- Involves humans for important approvals.

These are stages in our example to make the concept easy to follow. In a real application, RAG, tools and agentic behaviour can be combined in one system.

## 9. The central difference

Let's return to our opening question: **If AI can write an email, can it complete the hiring process?**

Now we can separate the capabilities:

- **Generative AI:** “Write the interview invitation email.”
- **RAG + Generative AI:** “Write it using our company's hiring policy and email template.”
- **Tools + Generative AI:** “Send the approved email through the email system.”
- **Agentic AI:** “Coordinate the hiring goal, track the process, notice what needs attention, and choose the next step using available information and tools.”

The difference is not that Agentic AI is simply a more advanced way to write an email. The difference is how the system's capabilities are organised.

**Generative AI is a capability: it creates content. Agentic AI is a goal-oriented way of coordinating capabilities and actions.**

An agentic system can use Generative AI to draft content, RAG to access relevant knowledge, and tools to perform actions. It can then use progress and results to coordinate the overall task.

So remember the hiring example: **writing the JD is one task; helping the hiring process move from the JD to onboarding is the larger goal.** That distinction is the main idea behind Generative AI vs Agentic AI.
