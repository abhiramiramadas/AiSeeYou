🚦 AiSeeYou
===========

**aka: “What if traffic cameras had anxiety and started overthinking everything?”**

An AI-based road accident detection system that watches traffic so humans don’t have to stare at CCTV footage like it’s a Netflix thriller.

Built for **traffic cameras**, not dashcams — because this system prefers to judge everyone equally from above.

💡 What is this?
----------------

AiSeeYou is my attempt at teaching a computer to answer the question:

> “Did that just… happen?”

It looks at traffic footage and:

*   tracks vehicles
    
*   calculates speed
    
*   watches distances like a helicopter parent
    
*   panics when cars get _too close for comfort_
    

If something looks even remotely suspicious, it goes:

**🚨 ACCIDENT DETECTED 🚨**

Sometimes correctly.Sometimes _emotionally early_.

👀 What it does (in human language)
-----------------------------------

*   Detects vehicles using YOLO (yes, the scary fast one)
    
*   Tracks them frame by frame
    
*   Estimates speed using pixel displacement (math happened, don’t ask)
    
*   Checks:
    
    *   sudden stops
        
    *   close proximity
        
    *   prolonged overlaps
        
*   Decides if the situation is:
    
    *   normal traffic
        
    *   risky behavior
        
    *   full-blown “something bad is about to happen”
        

Then it:

*   draws boxes
    
*   overlays speed
    
*   shouts **Accident Detected!** on screen
    
*   makes you question reality
    

🧠 Important Personality Trait of This System
---------------------------------------------

⚠️ **This model detects accident** _**risk**_**, not just post-accident wreckage.**

So yes:

*   It may alert **before** a visible crash
    
*   That’s not a bug
    
*   That’s ✨_predictive anxiety_✨
    

Think of it as:

> “Your mom yelling ‘slow down’ before anything happens.”

Thresholds are adjustable if you want it to calm down.

🧪 Tech Stack (for credibility)
-------------------------------

| Thing | Why it exists |
|------|---------------|
| Python | personality choice |
| YOLOv8 | because waiting is overrated |
| OpenCV | sees more than I do |
| NumPy | silent workhorse |
| Rule-based logic | because labeled accident datasets are a myth |
| Math | unfortunately unavoidable |
------------------------------------------
🗂️ Project Structure (mostly intentional)
------------------------------------------
## 🗂️ Project Structure (organized chaos)

```text
AiSeeYou/
│
├── Accident-Detection/
│   ├── detection.py        # where the paranoia lives
│   ├── alert.py            # screams internally
│   ├── config.py           # knobs to tune the anxiety
│   ├── main.py             # main character
│   ├── haversine-gui.py    # distance maths because earth is round
│   └── OSM.py              # maps, but optional
│
├── models/
│   └── (put YOLO weights here manually)
│
├── Requirements.txt
└── README.md
```

🐍 Setup (if you’re brave)
--------------------------
```
git clone https://github.com/abhiramiramadas/AiSeeYou.git
cd AiSeeYou
python -m venv venv
venv\Scripts\activate
pip install -r Requirements.txt
```

### Model Weights

Download YOLO weights (e.g. yolov8n.pt) and place them inside:
```
models/
```

They are **not** included because:

*   GitHub yelled at me
    
*   and honestly, fair

▶️ Running It
-------------
``` python Accident-Detection/main.py ```

You can tweak thresholds inside config.py if the system is:

*   too calm
    
*   too dramatic
    
*   behaving like it had coffee
    

📉 Known Issues (aka realism)
-----------------------------

*   Dense traffic = more false positives
    
*   Stationary vehicles sometimes get accused unfairly
    
*   Shadows occasionally scare the model
    
*   It does not understand:
    
    *   road rage
        
    *   human intent
        
    *   vibes
        

Yet.

🔮 Future Upgrades (if life allows)
-----------------------------------

*   ML-based accident classification (less guessing, more knowing)
    
*   Optical flow instead of raw pixel math
    
*   Lane awareness
    
*   Severity scoring (minor oops vs. oh no)
    
*   Emergency response integration
    

🤡 Why this project exists
--------------------------

*   Because traffic monitoring is boring
    
*   Because accidents are hard to label
    
*   Because “what if it _almost_ happened?” is more interesting
    
*   Because CCTV cameras deserve opinions too
    

👩‍💻 Author
------------

**Abhirami Ramadas**

Built with:

*   curiosity
    
*   frustration
    
*   and several Git mistakes (now resolved)
    

⭐ If you star this repo, the model might stop overreacting.No guarantees.
