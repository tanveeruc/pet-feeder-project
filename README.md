# Automated Pet Feeder Project

## Overview  
This project demonstrates the use of the **Problem-Solving Process** to design a low-cost, programmable **automated pet feeder** for an animal shelter.  
The feeder dispenses food for cats and dogs at scheduled times, monitors consumption, and alerts staff if food is not eaten or the container is empty.  
The project is structured into clear steps, from problem analysis to testing, and is documented in this repository.

---

## Features  
- Scheduled food dispensing (e.g., 8:00 AM, 6:00 PM)  
- Food level monitoring (full/low/empty)  
- Bowl weight tracking to detect pet consumption  
- Alerts for issues (food not dispensed, not eaten, hopper empty, door open)  
- Test cases to validate logic under different scenarios  
- Organised GitHub repository with diagrams, pseudocode, and outputs  

---

## Repository Structure  
/Step1_Analysis → Problem definition, requirements, system diagram
/Step2_Data → Inputs/outputs table, operational constraints
/Step3_Flowchart → Feeding logic flowchart (Draw.io, PNG/PDF)
/Step4_Word_Code → Word-based pseudocode implementation
/Step5_Testing → Test cases, outputs, CSV results
README.md → Project description and guide


---

## How It Works  
1. **Check schedule** → At feeding time, system verifies food availability.  
2. **Dispense food** → Servo motor rotates to drop portion into bowl.  
3. **Verify dispense** → Bowl weight increases after food is dropped.  
4. **Wait window** → After 10 minutes, check if bowl weight decreased.  
5. **Send alerts** → If food not dispensed, not eaten, or hopper empty.  
6. **Loop** → Repeat process for next scheduled time.  

---

## Test Scenarios  
- ✅ Pet eats as expected → No alert  
- ⚠️ Pet does not eat → “NOT_EATEN” alert  
- ⚠️ Food bin empty → “HOPPER_EMPTY” alert  
- ⚠️ Dispense failure → “DISPENSE_FAILURE” alert  
- ⚠️ Door open → “DOOR_OPEN” alert  
- ⚠️ Network down → Local buzzer/LED fallback  

---

## Future Improvements  
- Adaptive portion control based on pet size/weight  
- Mobile app integration for alerts and logs  
- Camera monitoring for visual confirmation  
- Low-battery and time-sync alerts  
- Health tracking from daily consumption logs  

---


