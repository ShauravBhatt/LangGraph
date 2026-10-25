# Lecture 2 — What Is Agentic AI?

*Balanced English + Hinglish notes*

## 1. Pehle basic idea samjho

**Agentic AI is an AI system that can take a goal from a user and work towards completing it with limited step-by-step human guidance.**

Simple words mein, normal chatbot ko tum ek-ek question poochte ho. Agentic AI ko tum ek **overall goal** dete ho, aur phir woh goal complete karne ke liye required steps figure out kar sakta hai.

For example:

- **Normal chatbot:** “Suggest some hotels in Goa.”
- **Agentic AI:** “Plan my Goa trip from the 15th to the 20th.”

Pehla chatbot hotels suggest karke ruk sakta hai. Agentic system travel options, hotels, places to visit aur itinerary jaise connected tasks par kaam kar sakta hai—provided uske paas required information aur tools available hon.

Agentic AI ke main behaviours hain: **planning, taking action, adapting to changes, and asking for help when needed.** Iska matlab ye nahi ki human involvement zero hota hai. Important decisions par human approval ab bhi zaroori ho sakta hai.

## 2. Reactive chatbot vs proactive agent

Goa trip ka example lete hain. Tum 15th se 20th tak Goa jaana chahte ho. Trip plan karne ke liye kaafi decisions lene padenge:

- Travel ka best option kya hai?
- Kahan stay karna chahiye?
- Kaun si places visit karni chahiye?
- Weather aur available time ke hisaab se itinerary kya ho?

### Normal Generative AI chatbot ke saath

Tumhe ek-ek karke questions poochne pad sakte hain:

1. “15th ko Goa pahunchne ka best way kya hai?”
2. “In dates ke liye hotels suggest karo.”
3. “Weather ke hisaab se kahan ghoomna chahiye?”
4. “Ab itinerary bana do.”

Chatbot har prompt ka answer deta hai, but process tum drive kar rahe ho. **This is reactive behaviour:** tum poochte ho, tab woh respond karta hai.

### Agentic AI system ke saath

Tum sirf overall goal de sakte ho:

> Plan a Goa trip for me from the 15th to the 20th.

Ab system connected tasks par khud kaam kar sakta hai, options research kar sakta hai aur itinerary bana sakta hai—agar uske paas required tools aur access hain.

**Yahi main difference hai:** you provide the goal, and the system figures out the steps needed to move towards it. Isse proactive, goal-oriented behaviour kehte hain.

## 3. Real-world example: AI hiring assistant

Ab ek detailed example lete hain. Imagine karo tum HR recruiter ho aur company ko **2–4 years experience wala remote Backend Engineer** hire karna hai. Tumhare paas ek Agentic AI assistant hai jo hiring process mein help karega.

### Step 1 — Goal samajhna aur plan banana

Tum assistant ko kehte ho:

> I want to hire a remote Backend Engineer with 2–4 years of experience.

System goal ko samajh kar ek possible plan banata hai:

1. Job description (JD) draft karna.
2. Suitable job platforms par JD publish karna.
3. Applications monitor karna.
4. Resumes screen karke suitable candidates identify karna.
5. Interviews schedule karna.
6. Interview questions prepare karne mein help karna.
7. Approval ke baad offer letter send karna.
8. Candidate accept kare toh onboarding start karna.

Notice karo, hiring ek single task nahi hai. Ye connected steps ki chain hai, aur kuch steps previous results par depend karte hain.

### Step 2 — Plan execute karna

JD banane ke liye assistant company documents use kar sakta hai, taaki usse pata chale:

- Engineer ko kaunsi technologies aani chahiye.
- Is experience level ki responsibilities kya hongi.
- Salary range kya hai.
- Company ki hiring requirements kya hain.

Assistant JD draft karke tumhe review ke liye deta hai. Tum approve kar do, toh woh next step par move kar sakta hai. **Woh sirf document generate karke rukta nahi; larger process ko aage badhata hai.**

### Step 3 — Tools use karke action lena

Assistant ke paas job platforms ki APIs ka access ho sakta hai. Required permissions ke saath woh approved JD publish kar sakta hai aur tumhe notify kar sakta hai ki job live ho gayi hai.

Phir woh applications monitor karta hai. Suppose three days baad sirf do candidates ne apply kiya.

System notice kar sakta hai ki applications expected number se kam hain. Woh suggest kar sakta hai ki JD revise karein ya job post ko promote karein. Changes karne se pehle woh tumhari approval maang sakta hai.

Approval milne ke baad, available tools se woh approved changes apply kar sakta hai.

**Yahan adaptability dikh rahi hai:** results achhe nahi aa rahe, toh system blindly same plan follow nahi karta; woh alternative suggest karta hai.

### Step 4 — Situation ke according process continue karna

Suppose ab applications aane lagti hain. Assistant:

- Resume parser se candidate details extract kar sakta hai.
- Resumes ko job requirements ke saath compare kar sakta hai.
- Shortlist suggest kar sakta hai—for example, two strong matches, three partial matches aur three weak matches.
- Tumse pooch sakta hai ki strong candidates ke interviews schedule kare?
- Calendar check karke available slots suggest kar sakta hai.
- Approval ke baad interview invitations send kar sakta hai.
- Interview ke din reminder aur relevant questions provide kar sakta hai.
- Company documents se offer letter draft kar sakta hai.
- Approved offer send karke acceptance status monitor kar sakta hai.
- Candidate accept kare toh welcome email, IT access request, laptop provisioning aur joining meeting jaise onboarding steps initiate karne mein help kar sakta hai.

Exact actions system ke tools aur permissions par depend karte hain. But overall idea ye hai ki assistant isolated questions ka answer dene ke bajay **hiring goal ke liye poore process ko coordinate** karta hai.

### Is example se kya notice karna chahiye?

Sabse striking feature hai **autonomy**. Tumne overall goal diya, aur system ne multiple steps plan aur execute kiye, with limited step-by-step guidance.

Saath hi, system results ke according adapt bhi kar sakta hai. Lekin publishing, spending money, ya offer send karne jaise important actions par human approval zaroori ho sakti hai.

Ab is practical example ko use karke Agentic AI ki key characteristics samajhte hain.

## 4. Agentic AI ki six key characteristics

Six important characteristics hain:

1. **Autonomy**
2. **Goal-oriented behaviour**
3. **Planning**
4. **Reasoning**
5. **Adaptability**
6. **Context awareness**

Inhe alag-alag samjhenge, but yaad rakho ki ye ek doosre se connected hain. For example, clear goal ke bina autonomy directionless ho sakti hai. Aur reasoning ke bina plan poor ho sakta hai.

## 5. Characteristic 1 — Autonomy

**Autonomy means an AI system can make decisions and take actions towards a goal without needing step-by-step human instructions.**

Hiring assistant ko tumne goal diya. Usne JD draft ki, approval ke baad publish ki, applications track ki aur next steps coordinate kiye. Tumhe har chhoti action ke liye separate instruction nahi deni padi.

### Autonomy kin forms mein dikh sakti hai?

- **Execution autonomy:** system planned steps ko one by one execute karta hai.
- **Decision-making autonomy:** resumes assess karke strong aur weak candidate matches identify kar sakta hai.
- **Tool-use autonomy:** decide kar sakta hai ki current task ke liye kaunsa available tool use karna chahiye—for example, interview schedule karne ke liye calendar API.

Toh autonomy ka matlab sirf fixed steps ko automatically execute karna nahi. System situation ke according actions aur tools choose bhi kar sakta hai.

### Kya agent ko unlimited freedom de deni chahiye?

Bilkul nahi. Too much autonomy risky ho sakti hai:

- Wrong salary ya terms ke saath offer send ho sakta hai.
- Candidate screening mein bias aa sakta hai.
- Agent bina approval ke job ads par unnecessary money spend kar sakta hai.

Isliye autonomy ko control karna important hai.

### Autonomy control karne ke ways

- **Limit permissions:** decide karo ki agent independently kya kar sakta hai. For example, resumes screen kar sakta hai, but candidate reject karne se pehle approval chahiye.
- **Human-in-the-loop checkpoints:** sensitive actions se pehle human approval required rakho, jaise JD publish karna ya offer send karna.
- **Human override:** user agent ko pause, stop ya redirect kar sake. Example: “Pause hiring.”
- **Guardrails and policies:** clear rules define karo, jaise weekends par interviews schedule nahi karne ya professional language use karne ka rule.

Aim ye hai ki agent useful amount of freedom ke saath kaam kare, but risky decisions uncontrolled na hon.

## 6. Characteristic 2 — Goal-oriented behaviour

**A goal-oriented system keeps its actions directed towards a continuing objective instead of responding only to isolated prompts.**

Hiring example mein main goal hai suitable Backend Engineer hire karna. JD draft karna, publish karna, resumes screen karna aur interviews schedule karna—all of these actions isi goal ko support karte hain.

### Autonomy aur goal ka connection

- **Autonomy asks:** “Can the system act on its own?”
- **Goal asks:** “What should those actions achieve?”

Goal, autonomy ke liye compass ki tarah kaam karta hai. Agar clear goal nahi hoga, toh system actions toh le sakta hai, but zaroori nahi ki woh desired result ki taraf le jaayein.

### Goals ke saath constraints bhi ho sakte hain

- Hire a Backend Engineer.
- Remote role ke liye hire karo.
- Candidate ke paas 2–4 years ka experience ho.
- Hiring budget ke andar rehna hai.
- Particular technical skills required hain.

Constraints batate hain ki acceptable result kaisa hona chahiye.

### Goal ke saath progress bhi track honi chahiye

System relevant information maintain kar sakta hai:

- **Main goal:** Backend Engineer hire karna.
- **Constraints:** remote role, 2–4 years experience, required skills.
- **Current status:** active ya completed.
- **Progress:** JD drafted, job posted, applications received, interviews scheduled.
- **Remaining tasks:** candidate select karna aur onboarding complete karna.

Ye sirf conceptual representation hai; actual system goal aur progress ko different formats mein store kar sakta hai.

Ek aur useful point: goal midway change ho sakta hai. Suppose suitable applications nahi aa rahi aur company decide karti hai ki full-time engineer ke bajay freelancer hire karna hai. Ab agent ko goal update karke plan bhi change karna padega.

## 7. Characteristic 3 — Planning

**Planning is the ability to break a high-level goal into a structured sequence of actions or smaller sub-goals.**

“Hire a Backend Engineer” ek broad goal hai. Isko execute karne ke liye system smaller steps banata hai—JD draft karna, job publish karna, applications screen karna, interviews schedule karna, etc.

Planning aur execution connected hain:

1. **Planning:** decide karna ki kya karna hai aur kis order mein.
2. **Execution:** selected steps perform karna.
3. **Re-planning:** agar koi step fail ho jaaye ya situation change ho, toh plan revise karke continue karna.

Ye cycle goal achieve hone tak repeat ho sakti hai, ya jab human help ki need ho.

### Sirf ek plan kyun nahi?

Agent multiple possible plans consider kar sakta hai. Hiring ke liye do possible options:

- **Plan A:** job portals par JD publish karo aur post promote karo.
- **Plan B:** internal referrals use karo ya hiring agency approach karo.

Dono ka goal same hai, but cost, speed, risk aur candidate reach different ho sakti hai.

### Best plan kaise choose hoga?

System possible plans ko different factors par evaluate kar sakta hai:

- **Efficiency:** kaunsa plan faster ho sakta hai?
- **Tool availability:** required tools available hain ya nahi?
- **Cost:** kaunsa option budget mein fit hota hai?
- **Risk:** kis plan ke fail hone ya problem create karne ke chances zyada hain?
- **Constraints:** kaunsa plan remote hiring jaise requirements ko better match karta hai?

Evaluation ke baad system suitable plan select karta hai. Decision predefined policy ke basis par ho sakta hai ya human input liya ja sakta hai.

So planning ko three-part process ke roop mein yaad rakho:

1. Multiple plans generate karo.
2. Plans evaluate karo.
3. Best suitable plan select karke execute karo.

Aur agar selected plan kaam nahi karta, toh agent wapas planning par jaake alternative choose kar sakta hai.

## 8. Characteristic 4 — Reasoning

**Reasoning is the process of interpreting information, drawing conclusions, and making decisions.**

Reasoning planning aur execution dono mein needed hai. Planning mein decide hota hai ki kya karna chahiye; execution mein decide karna pad sakta hai ki unexpected situation aaye toh next step kya ho.

### Ek simple human example

Suppose tumhara phone chori ho gaya:

1. Tum notice karte ho ki phone missing hai.
2. Tum conclude karte ho ki phone chori hua ho sakta hai.
3. Tum realise karte ho ki koi tumhara number misuse kar sakta hai.
4. Tum mobile provider ko call karke number block karne ka decision lete ho.

Tumne information interpret ki, conclusion nikala aur action choose kiya. AI agent ko bhi feedback samajhkar conclusion aur action decide karna hota hai.

### Planning ke time reasoning

- **Goal breakdown:** hire karne ke goal ke liye kaun-kaun se steps required hain?
- **Tool selection:** resumes analyse karne ke liye resume parser aur interview scheduling ke liye calendar API useful hai.
- **Resource estimation:** kitna time, money ya access required hoga? Kaun se steps ek doosre par depend karte hain?

### Execution ke time reasoning

- **Decision-making:** agar three candidates suitable lag rahe hain, toh two ko interview ke liye recommend karein ya all three ko?
- **Human help:** salary information clear nahi hai, toh available sources search karein ya recruiter se poochhein?
- **Error handling:** job platform down hai, toh retry karein, another approved platform use karein, ya recruiter ko inform karein?

Reasoning ki wajah se agent situation ke according decision le sakta hai, instead of blindly same action repeat karne ke.

## 9. Characteristic 5 — Adaptability

**Adaptability is the ability to modify plans, strategies, or actions when unexpected conditions arise, while still working towards the goal.**

Hiring assistant ko yaad karo: JD publish karne ke three days baad sirf two applications aayi. System ne JD revise karne ya post promote karne ka suggestion diya. Ye adaptability hai—current approach expected result nahi de rahi, so agent alternative consider karta hai.

### Agent ko adapt kab karna pad sakta hai?

- **Tool failure:** calendar API unavailable hai, toh agent recruiter se availability pooch sakta hai instead of getting stuck.
- **Unexpected feedback:** applications bahut kam aa rahi hain, toh agent JD ya promotion strategy change karne ka suggestion de sakta hai.
- **Goal change:** company full-time engineer ke bajay freelancer hire karna chahti hai, toh plan bhi update hoga.

Yahan **environment** ka matlab hai woh real-world setting jahan agent kaam karta hai—for example, job platforms, applicants, recruiter, calendar aur connected systems.

Adaptability ka matlab randomly direction change karna nahi hai. Agent ko new information ke basis par approach adjust karni chahiye, while keeping the goal and its constraints in mind.

## 10. Characteristic 6 — Context awareness

**Context awareness means understanding and using relevant information from the current task, earlier interactions, user preferences, and the environment.**

Hiring process days ya weeks tak chal sakta hai. Imagine karo tumne JD publish karwai, aur four days baad poochha: “How many people have applied?”

Agar assistant original task aur progress bhool gaya, toh usse pata hi nahi hoga ki tum kis job ki baat kar rahe ho. Long-running process coordinate karne ke liye relevant context maintain karna important hai.

### Agent ko kaunsa context yaad rakhna chahiye?

- **Original goal:** system ko achieve kya karna hai.
- **Progress:** kaun se tasks complete hain aur kaun se pending.
- **Conversation:** pehle kya instructions, decisions aur approvals mile.
- **Environment state:** job publish hui ya nahi, kitni applications aayi, ad budget kitna bacha.
- **Tool results:** resume parser ya calendar API se kya information mili.
- **User preferences:** recruiter remote candidates prefer karta hai ya interview questions Google Doc mein chahta hai.
- **Policies and guardrails:** offer letter human approval ke bina send nahi karna.

Ye context agent ko process continue karne mein help karta hai, rather than har interaction ko ek completely new task samajhne ke.

### Short-term vs long-term memory

Memory context maintain karne ka ek way hai. Broadly, do useful types hain:

- **Short-term memory:** current session ya task ki recent messages, tool results aur immediate decisions.
- **Long-term memory:** information jo future sessions mein bhi useful rahe, jaise stable user preferences, past interactions aur persistent rules.

For example, kisi candidate ke resume parser ka result current hiring task ka short-term information ho sakta hai. “Offer send karne se pehle human approval required hai” ek persistent rule ho sakta hai jo long-term mein retain karna useful hai.

Actual implementation system ke according vary karti hai, but core idea same hai: **context ke bina agent ko har baar zero se start karna padega; context ke saath woh task ko intelligently continue kar sakta hai.**

## 11. Agentic AI ke five high-level components

Ab tak humne dekha ki agentic system **kaise behave karta hai**—autonomy, goals, planning, reasoning, adaptability aur context awareness ke through.

Next question: **system ke andar kaun se major parts milkar ye behaviour support karte hain?**

Ek typical LLM-based agentic application ko five high-level components se samajh sakte hain:

1. Brain
2. Orchestrator
3. Tools
4. Memory
5. Supervisor

Real systems mein additional components bhi ho sakte hain, but ye five ek useful high-level picture dete hain.

## 12. Component 1 — Brain

LLM-based agentic application mein **brain generally Large Language Model (LLM)** hota hai. Ye interpretation aur decision-making ke kaafi parts handle karta hai.

Brain can:

- **Interpret the goal:** user actually achieve kya karna chahta hai, usse samajhna.
- **Help with planning:** goal ko smaller tasks mein break karna.
- **Reason:** available information interpret karke sensible decision suggest karna.
- **Select tools:** current task ke liye suitable tool choose karna.
- **Communicate:** user messages samajhna aur natural-language responses generate karna.

Hiring assistant mein brain goal samajhne, process plan karne, resume parser ki need identify karne aur recruiter ko progress explain karne mein help karta hai.

Simple way mein, brain figure out karta hai **kya hona chahiye aur kyun**.

## 13. Component 2 — Orchestrator

**Orchestrator plan ke execution ko coordinate karta hai.** Brain plan suggest kar sakta hai, but orchestrator ensure karta hai ki steps right order mein run hon aur results ke according next step choose ho.

Iske common responsibilities hain:

- **Task sequencing:** steps ka order manage karna.
- **Conditional routing:** result ke according next step select karna. For example, suitable candidates milne par interviews ki taraf jaana; applications kam hon toh hiring strategy revisit karna.
- **Retries:** temporary tool failure par dobara try karna.
- **Loops and iteration:** zaroorat padne par step repeat karna.
- **Delegation:** task ko right system component tak route karna ya human ko involve karna.

Orchestrator ko project manager ki tarah samjho jo different steps coordinate karta hai. Isse system sirf plan banata nahi, balki actual execution bhi aage badhata hai.

LangGraph jaise frameworks orchestration build karne mein use ho sakte hain, but yahan main focus orchestrator ke role par hai—not framework implementation.

## 14. Component 3 — Tools

**Tools agent ko external systems ke saath interact karne aur actions perform karne ki ability dete hain.** Appropriate tools ke bina system action suggest toh kar sakta hai, but outside world mein action perform nahi kar payega.

Examples:

- Job publish karne ke liye APIs.
- Candidate information extract karne ke liye resume parser.
- Interview schedule karne ke liye calendar tools.
- Emails send karne ke liye email tool.
- Hiring information update karne ke liye database ya HR system.

Company knowledge base se information retrieve karne ka mechanism bhi agent ko tool ke through available karwaya ja sakta hai.

Yaad rakhne ka simple way: **brain decide karta hai kya karna useful ho sakta hai; tools actual action perform karne ki capability dete hain.** Action tabhi possible hai jab tool aur required permissions available hon.

## 15. Component 4 — Memory

Memory woh information store karti hai jise agent ko baad mein use karna hai. Ye context awareness aur task progress maintain karne mein help karti hai.

- **Short-term memory:** recent messages, tool outputs aur current task ke decisions.
- **Long-term memory:** stable preferences, previous interactions aur persistent rules.
- **Progress tracking:** kaun se steps complete hue aur kya pending hai.

Hiring example mein memory retain kar sakti hai ki JD publish ho chuki hai, eight applications aayi hain, two interviews schedule hain aur offer abhi approval ka wait kar raha hai.

Agar ye information available nahi hogi, toh agent completed work repeat kar sakta hai ya pending step miss kar sakta hai.

## 16. Component 5 — Supervisor

**Supervisor human-in-the-loop behaviour ko support karta hai.** Ye ensure karne mein help karta hai ki approval, oversight ya escalation required ho toh human ko involve kiya jaaye.

Supervisor useful hai jab:

- **Approval required ho:** offer send karne ya ads par money spend karne se pehle recruiter se permission leni ho.
- **Guardrail enforce karna ho:** restricted action approval ke bina proceed na kare.
- **Unusual situation aaye:** case normal rules se match nahi karta aur human judgement needed ho.

For example, screening rules ke according ek candidate perfect match na lage, but resume mein kuch unusual strong experience ho. Agent ko silently final decision lene ke bajay case human review ke liye escalate karna chahiye.

Supervisor ka purpose autonomy ko eliminate karna nahi, balki **autonomy ke saath appropriate oversight maintain karna** hai.

## 17. Five components milkar kaise kaam karte hain?

Hiring assistant ke through sabko connect karte hain:

1. **Brain:** goal samajhta hai aur plan suggest karta hai.
2. **Orchestrator:** steps coordinate karta hai aur results ke according next step choose karta hai.
3. **Tools:** JD publish karte hain, resumes parse karte hain, calendars check karte hain ya approved emails send karte hain.
4. **Memory:** goal, conversation, tool results, decisions aur progress retain karti hai.
5. **Supervisor:** approvals, guardrails aur unusual cases mein recruiter ko involve karta hai.

Ye five unrelated boxes nahi hain. Ye saath milkar pehle discuss ki hui characteristics ko support karte hain.

For example, **goal orientation** ke liye objective track karna zaroori hai. **Planning and reasoning** decide karne mein help karte hain ki kya karna chahiye. **Orchestrator** execution coordinate karta hai, **tools** external actions enable karte hain, **memory** context retain karti hai, aur **supervisor** human oversight provide karta hai. Results expected na hon toh agent reasoning aur adaptability use karke approach revise kar sakta hai.

## 18. Bringing the whole idea together

Agentic AI sirf isliye agentic nahi ho jaati kyunki woh LLM use karti hai ya uske paas tools hain. Important ye hai ki system in capabilities ko **ek goal achieve karne ke liye kaise coordinate** karta hai.

Six key characteristics yaad rakho:

- **Autonomy:** constant step-by-step instructions ke bina appropriate actions lena.
- **Goal orientation:** actions ko objective ki direction mein rakhna.
- **Planning:** goal ko smaller steps mein todna aur possible paths consider karna.
- **Reasoning:** information interpret karke decisions lena.
- **Adaptability:** unexpected situations ya changed goals ke according adjust karna.
- **Context awareness:** relevant information aur progress ko use karna.

Aur high level par, brain, orchestrator, tools, memory aur supervisor milkar is behaviour ko support karte hain.

Hiring example par wapas aao. Normal chatbot poochhne par JD draft kar sakta hai. Agentic hiring assistant larger goal par kaam karta hai: hiring plan banana, tools se steps execute karna, progress track karna, applications kam hon toh approach adapt karna, aur important approvals ke liye recruiter ko involve karna.

**Yahi Agentic AI ka core idea hai: planning, decisions, actions aur context ko coordinate karke ek goal ki taraf kaam karna—with appropriate human oversight.**
