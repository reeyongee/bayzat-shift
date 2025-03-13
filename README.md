# Designing a Shift Swap Solution for Bayzat
## Chapter 1: Disclaimer

#### _This isn’t an official Bayzat project—it’s a personal endeavor, born from my drive to join their team as an Associate Product Manager. I’m not on their payroll or peeking behind their curtains; everything here comes from my own exploration, fueled by a mix of curiosity and ambition._  

Think of it as my calling card to Safwan and the Bayzat crew—a way to show what I can bring to the table. I’ve poured my heart into this, not because I was asked, but because I see Bayzat as a place where I can grow, contribute, and make a dent. So, while the ideas ahead are mine alone, they’re crafted with Bayzat’s world in mind—hoping to catch their eye and spark a conversation.

## Chapter 2: Storytime: The Road to Bayzat 

I’m Aakash Nair 👋, an engineer by training who’s now all-in on product management—and Bayzat’s where I want to land. I graduated with a Bachelor’s in Electronics & Communication from Manipal Institute of Technology, ready to tackle the world, until a bike accident flipped the script. For 18 months, I was bedridden—disconnected from my ambitions, wrestling with setbacks. It was rough, but it lit a fire: I’d come back stronger, chasing a career that blends tech, creativity, and real impact. Fast forward to now—I’m in Dubai, visa on its last legs, funds running thin, and holding a QA testing offer from a past gig. Solid, sure, but product management’s my heart, and Bayzat’s fresher-friendly, remote role feels like my shot.


<p align="center">
  <img src="https://github.com/user-attachments/assets/e9b8ec4e-88c5-4066-b534-98c04ede9350" width="250">
</p>
<p align="center"><em style="font-size: 10px;">A picture of me after my last job interview in Dubai.</em></p>


To stand out, I decided to dig into Bayzat’s app and dream up something cool—my way of saying, “Hey, Safwan, I get it.” I logged in to both the iOS and Android versions of the app, but I couldn't get the demo section of the app running on either (Maybe it's something that's still under construction?). Then I spotted their demo video online—perfect, except it was locked behind a form that only accepted a corporate email. Unemployed me didn’t have one handy, so I got crafty: spoofed a temp-mail and signed in to sneak a peek (maybe something to look out for as a product manager? 👀). It worked—I got a glimpse of Bayzat’s sleek UI: Home, Work, Health, Perks, My Profile tabs, all polished and promising.


<p align="center">
  <img src="https://github.com/user-attachments/assets/95117af0-d6f7-4813-a789-6e0d543ae938" width="500">
</p>
<p align="center"><em style="font-size: 10px;">Putting in the fake details with a temp mail address just in case there was a verification link sent to it.</em></p>


That’s when it hit me. Shift swapping—a feature I’d need if I were juggling retail or healthcare shifts in the UAE—felt like it could use a boost. The video showed schedules under “Work,” but swapping? Either buried or clunky, it didn’t scream “quick fix.” With my back against the wall, I saw a chance. Bayzat’s data-rich platform could handle this; it just needed a nudge. So, I set out to design a one-tap shift swap—my ticket to show Bayzat I’m not just another applicant, but someone who can spot a gap and fill it.

## Chapter 3: Defining the Problem 🎯

After spotting the shift swap gap in Bayzat’s demo, I started with: “Swapping shifts in this app isn’t intuitive.” I needed to zoom out. Was this just me, or a real snag for Bayzat’s users? So, I redefined it: “Bayzat users encounter friction when swapping shifts, a pain point for shift workers in markets like the UAE where schedules rule.” 🔄

The wheels started turning. Why do people even swap shifts? Emergencies pop up—sick kid, flat tire—or maybe it’s just a better day off. What’s the current flow like? From the demo, it’s likely tucked under the Work tab, maybe a manual ping to a teammate or manager—too many steps for a crunch. How’s the competition handling this? I’d peeked at Deputy’s multi-step swap process—functional, but not fast. Could Bayzat leap ahead? And what’s Bayzat’s edge here? The UAE’s retail (**Jimmy Choo** 👀), healthcare, and hospitality (**Fuchsia Restaurant** 👀) scenes thrive on shift workers—flexibility could be a game-changer in this region. 🚀

Just because I couldn’t find the swap button didn’t mean it was a universal headache. _I’m not the user; I’m designing for them._ Shift workers—nurses pulling doubles, cashiers dodging rush hour—need this to work seamlessly, not just for my demo woes. That shift in mindset turned my curiosity into a challenge: pinpoint the friction and fix it. Bayzat’s got the bones—schedules, teammate data—so why not make swapping as easy as ordering takeout? 🍔 That’s where I landed: a problem worth solving, if I could crack it right.

## Chapter 4: Breaking Down the Shift Swap Experience 🔍

With the problem framed, I turned to what Bayzat’s shift swap experience might actually look like—or at least, what I could piece together from the demo video. The glimpse I got showed a clean “Work” tab with shift schedules laid out—dates, times, roles—but swapping? That was a blank spot. My best guess: it’s either buried somewhere in there or relies on a clunky workaround, like messaging a teammate and hoping a manager sorts it out. For a nurse racing against a morning handover or a cashier dodging a peak-hour clash, that’s not cutting it. ⏱️

First snag: visibility. If swapping’s an option, it’s not waving at you. The Work tab screamed schedules, not solutions—nothing said “swap this now.” I’d bet it’s a few taps deep, if it’s there at all, and that’s a miss when seconds count. Second issue: efficiency. A multi-step process—find shift, contact someone, wait—drags out what should be instant. In a pinch, shift workers need a lifeline, not a scavenger hunt. 🚨

But here’s the kicker: This isn’t a data problem; it’s a UI one. Swapping shift fields in the existing schema could turn a chore into a breeze. 🌬️

Observation: speed matters—shift swaps are clutch moments. User empathy: imagine the stress of a last-minute conflict; workers need a quick out. Solution insight: a one-tap fix could harness Bayzat’s data without breaking a sweat. Then came the spark—placement. Quick Links on the Home tab could scream “emergency swap,” perfect for that 8 AM panic. But keeping it in Work makes sense too—context is king for routine swaps. Why pick? Dual access could cover both worlds—urgent and planned. It’s a small tweak, but it could shift the game for Bayzat’s users, and I was itching to test the hunch.

## Chapter 5: Research: The Bigger Picture 🌐

To ground my hunch about Bayzat’s shift swap potential, I scoped out the competition. Deputy’s a big player—its swap flow lets you pick a teammate, send a request, and wait for approval. It works, but it’s a slog—multiple steps when you’re racing the clock. BambooHR sticks to scheduling basics; swapping’s barely a whisper. Gusto’s all about employee perks, not shift juggling—it’s playing a different game. The takeaway? Competitors aren’t nailing this. Deputy’s closest, but it’s not fast or frictionless. Bayzat, with its Middle East focus, could leap ahead—turn a clunky process into a sleek edge. 🚀

Social media and app reviews were trickier—Bayzat’s specifics were sparse, thanks to my demo access woes. But digging through Twitter and app stores, I found a pattern: HR app users gripe about rigid schedules and slow fixes. “Why can’t I just swap this shift?” one tweet moaned. It’s not Bayzat-specific, but the sentiment fits—shift workers want control, and they’re not getting it. 🗣️



<div style="display: flex; justify-content: center; gap: 1000px;">
  <img src="https://github.com/user-attachments/assets/ae7fe760-52e1-4dd9-baa8-7e3ce4c1773b" width="45%">
  <img src="https://github.com/user-attachments/assets/16f78dd4-e632-47f1-8830-d6b8a38fd36f" width="45%">
</div>
<p align="center"><em>Shoutout to ChatGPT for being my personal translator. 😂</em></p>



That lit a bulb. Bayzat’s already got the goods—schedules, teammate data, hours—locked and loaded. This isn’t about building new pipes; it’s about unclogging the flow. With no Bayzat users to interview, I leaned on imagination, channeling 10 UAE shift workers—retail clerks, nurses, delivery drivers. I pictured sitting with them, coffee in hand, asking: “How do you swap shifts now? What’s the headache?” ☕

The answers I conjured weren’t shocking. “Swaps? It’s WhatsApp or bust—pinging teammates, praying someone bites,” a cashier might say. “Takes forever, and half the time, it falls apart,” a nurse could add. Managers likely groan too: “I’m stuck playing middleman—emails, calls, chaos.” Friction’s the theme—slow, messy, manual. What’s the dream? “Show me who’s free, let me tap once, done.” Speed, control, less hassle—shift workers want a lifeline, not a labyrinth. 💡

## Chapter 7: The Solution: One-Tap Shift Swap

My solution? A “Swap Shift” feature, slotted into Quick Links on the Home tab and the Work tab, powered by Bayzat’s existing data—no heavy lifting required. It’s a UI layer tweak, not a backend beast. Schedules, teammate roles, hours—it’s all there, the goal: swap shift fields with one tap, keeping users and managers sane. 
Here’s the flow. 


![image](https://github.com/user-attachments/assets/bed0788f-06ba-4da1-abc3-d8bbf92723b8)




__Screen 1__: Home—the Quick Links section on the Home tab sports a “Swap Shift” tile, right alongside the other links for a last-minute crunch.


<p align="center">
  <img src="https://github.com/user-attachments/assets/c4866d85-6efe-4088-89fa-5188c9576f76" width="250">
</p>
<p align="center"><em style="font-size: 10px;">Quick Links section with the "Swap Shift" tile for last-minute changes.</em></p>


__Screen 2__: Shift Selection—your upcoming shifts pop up (e.g., “Mon, Mar 12 | 9:00 AM - 5:00 PM | Cashier - Dubai Mall”), each with a profile icon hinting at swap options and a “Swap” button. Pick one—say, that Monday slot. 


<p align="center">
  <img src="https://github.com/user-attachments/assets/e23b8097-5330-4256-a978-e762eea693b6" width="250">
</p>
<p align="center"><em style="font-size: 10px;">Shift Selection screen showing available shifts and swap options.</em></p>   


__Screen 3__: Swap Pop-Up—a modal lists teammates with matching shifts (e.g., “Safwan Youseph | 1:00 PM - 9:00 PM”), profile icons included, and a “Request” button. Tapping on it expands a card with the option to call the person you intend to swap with to talk to them, the Request Swap button is displayed alongside it and is now enlarged. Tap it, and the request fires off. Post-Request—you’re back on Screen 2, the shift now tagged “Pending.” Teammates see “Accept/Decline” in their notifications pane; managers get “Approve/Reject” in theirs—no extra screens cluttering the app.


<table align="center">
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/7f76424a-1cc3-4970-a547-225501c3d3d5" width="250">
      <br>
      <em style="font-size: 10px;">Swap pop-up displaying available teammates with matching shifts.</em>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/f39c9392-f489-40a2-81ed-6f689fb20ecc" width="250">
      <br>
      <em style="font-size: 10px;">Expanded swap request card with call and request options.</em>
    </td>
  </tr>
</table>


__Screen 4__: Receiver’s Notification—Safwan’s phone pings: “Sarah Ahmed wants to swap shifts with you.” There's “Accept” (purple) and “Reject” (gray) buttons, shift details stacked for clarity. They tap; it’s done—no app detour.


<p align="center">
  <img src="https://github.com/user-attachments/assets/38b6078a-a5ae-4a24-bf96-061c12077def" width="250">
</p>
<p align="center"><em style="font-size: 10px;">Receiver's notification showing the shift swap request.</em></p>


__Screen 5__: Manager’s Notification—the manager sees: “Shift Swap Request: Safwan Youseph and Sarah Ahmed" along with the dates and the times. Icons for both, “Approve” (purple) or “Reject” (gray). Bayzat’s backend handles it, no screen bloat.


<p align="center">
  <img src="https://github.com/user-attachments/assets/94769335-20e2-42ea-be48-18d9ca311563" width="250">
</p>
<p align="center"><em style="font-size: 10px;">Manager's notification for approving or rejecting the shift swap.</em></p>


It’s lean by design. Bayzat’s data does the heavy lifting—matching shifts, flagging eligible teammates—while the UI keeps it snappy. And here’s a twist: the logic can flex for cross-day swaps. Say you can’t work March 14 but want March 15—find someone free on 14 to take your shift. Same framework, minor tweak, all within the existing schema. No new tables, just smarter field swaps.

I debated feature placement hard—Quick Links screams “now!” for that 8 AM panic, but Work keeps it grounded for planned swaps. Dual access won out—why force a choice when both fit?

_Observation_: Shift swaps need speed—Bayzat’s data’s ready, just not front-facing. _User Empathy_: Workers juggling life deserve a break—suggestions cut the chaos. _Solution Insight_: One-tap harnesses what’s there—Quick Links for urgency, Work for context, notifications for approvals. _Value Add_: Bayzat could own this space—Deputy’s multi-step slog can’t touch it. 

## Chapter 10: Conclusion: Reflections and Next Steps

This project began as a personal challenge—to explore Bayzat’s potential through a shift swap feature—and evolved into a demonstration of what I could contribute as an Associate Product Manager. For me, this is more than a design—it’s a statement of intent.

Looking ahead, I’d welcome the chance to discuss this with Safwan and the Bayzat team, ideally in person once I’m back in Dubai with my visa renewed. My goal isn’t just to join—it’s to contribute, learn, and grow alongside a team shaping HR solutions. This project is my first step; I’m ready to take the next with Bayzat. If you made it this far I wanna express my deepest gratitude for your time and consideration. It means more to me than words can fully capture to have this effort reviewed. Your attention to my journey and ideas is genuinely appreciated, and I’m honored to share this with you.

__Thank you.__
