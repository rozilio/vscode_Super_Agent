1. פתיחת פרויקט חדש \ CLONE או עבודה בפרויקט קיים.
2. העתקת קובץ main.instructions.md לתיקיה -  "C:\<YOUR_PROJECT_DIRECTORY>\.github\instructions\" (אם הנתיב לא קיים, צרו את הנתיב).
3. ב-PLAN MODE לתת את הפקודה - initialize memory bank and create all the core and optional files
4. לעבור ל- ACT MODE ולאשר.

אופציה ב - 
1. להעתיק את קובץ ההוראות הראשי לנתיב - "C:\<YOUR_PROJECT_DIRECTORY>\.github\instructions\" (אם הנתיב לא קיים, צרו את הנתיב).
2. להעתיק את תיקיית Memory-Bank לנתיב - "C:\<YOUR_PROJECT_DIRECTORY>\".
3. ההיררכיה תראה כך - 
<YOUR_PROJECT_DIRECTORY> 
├── memory-bank/
     ├── projectbrief.md          (Foundation - created first)
     ├── productContext.md        (Built from projectbrief)
     ├── systemPatterns.md        (Built from projectbrief)
     ├── techContext.md          (Built from projectbrief)
     ├── activeContext.md        (Built from above three)
     ├── progress.md             (Built from activeContext)
     └── tasks/
         └── _index.md           (Task management system)
