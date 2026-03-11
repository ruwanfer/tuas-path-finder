# 🎓 TUAS ICT Competence Path Finder

**Turku University of Applied Sciences - Find Your Ideal Specialization Path**

![Version](https://img.shields.io/badge/version-1.0.0-blue)
![Status](https://img.shields.io/badge/status-stable-green)
![TUAS](https://img.shields.io/badge/TUAS-ICT%20Student%20Tool-orange)

##  About The Project

This tool helps first-year ICT students at **Turku University of Applied Sciences** choose their competence path for years 2-4. Based on your:

- **📚 First-year subject grades** (70% of recommendation)
- **💡 Personal interests** (15% of recommendation)
- **🔧 Current technical knowledge** (15% of recommendation)

The algorithm analyzes your profile and suggests which of the six competence paths best matches your strengths and interests.

###  The Six Competence Paths

| Path | Focus Area |
|------|------------|
| **Data Engineering and AI** | Big data, machine learning, analytics |
| **Data Networks and Cybersecurity** | Network infrastructure, security, protocols |
| **Embedded Software and IoT** | Hardware programming, sensors, smart devices |
| **Game and Interactive Technologies** | Game design, VR/AR, interactive media |
| **Health Technology** | Medical devices, health informatics, biotech |
| **Software Engineering and Project Management** | App development, team leadership, agile |

---

##  Features

- ✅ **TUAS-specific** - Uses actual first-year curriculum subjects
- ✅ **70% grade-based** - Recommendations heavily weighted by your academic performance
- ✅ **Comprehensive analysis** - Evaluates 13 subjects + 28 interests + 49 technical skills
- ✅ **Visual results** - Color-coded match percentages with detailed breakdowns
- ✅ **Mobile responsive** - Works on phones, tablets, and computers
- ✅ **Instant feedback** - Get recommendations immediately after rating yourself

---

##  Live Demo

**Try it here:** https://github.com/ruwanfer/tuas-path-finder

---

##  How to Use

### For Students (Using the Tool)

1. **Open the tool** in your browser
2. **Rate yourself** in three categories (all on scale 1-5):
   - **First Year Subjects**: Enter your actual grades
   - **Personal Interests**: How much you're interested in each area
   - **Technical Knowledge**: Your current skill level

3. Click **"Find My Best Path"**
4. View your results:
   - 🟢 **Green cards** (70%+) = Strong match
   - 🟡 **Yellow cards** (50-69%) = Good match
   - 🔴 **Red cards** (below 50%) = Consider other paths

5. Use the breakdown to understand why each path was recommended

### Example Rating Scale

| Rating | Meaning |
|--------|---------|
| 5 | Excellent / Very interested / Expert |
| 4 | Good / Interested / Proficient |
| 3 | Average / Neutral / Intermediate |
| 2 | Below average / Not interested / Beginner |
| 1 | Poor / Not interested at all / No knowledge |

---

##  For Developers

### Project Structure
```
tuas-path-finder/
│
├── index.html          # Main application file
├── README.md           # This documentation
└── (no other files needed - it's all in one HTML!)
```

### Key Technologies
- HTML5
- CSS3 (Flexbox/Grid for responsive design)
- Vanilla JavaScript (no frameworks)

### How the Algorithm Works

```javascript
// Weight distribution
const weights = {
    subjects: 0.7,   // 70% based on grades
    interests: 0.15,  // 15% based on interests
    knowledge: 0.15   // 15% based on current skills
};

// For each path, we calculate:
match_score = (subject_match * 0.7) + 
              (interest_match * 0.15) + 
              (knowledge_match * 0.15)
```

Each competence path has pre-configured **importance weights** for every subject, interest, and skill. These weights were determined based on:
- TUAS curriculum documents
- Industry requirements
- Feedback from senior students and teachers

---

##  Data Sources

The subject list is based on the actual **TUAS ICT first-year curriculum**:

- Mathematics (General)
- Calculus
- Engineering Precalculus
- Topics in Applied Mathematics
- Measurement in Physics
- Engineering Physics
- Introduction to Electronics
- Introduction to Programming
- Databases
- Git Basics
- Low-Code Software Development
- Introduction to IT
- Project Work Basics

---

##  Contributing

Found a bug? Have a suggestion? Want to improve the weightings?

1. **Fork the repository**
2. Create your feature branch: `git checkout -b feature/YourImprovement`
3. Commit your changes: `git commit -m 'Add some improvement'`
4. Push to the branch: `git push origin feature/YourImprovement`
5. Open a Pull Request

Or simply **open an issue** with your feedback!

---

##  License

This project is created for educational purposes at **Turku University of Applied Sciences**. Feel free to use, modify, and share with fellow students.

**© 2024 TUAS ICT Student Project**

---

##  Contact

**Created by:** [Ruwan Gammanage]
-  Email: ruwan.gammanage@edu.turkuamk.fi
-  Student: ICT Engineering, Turku University of Applied Sciences
-  GitHub: [@ruwanfer](https://github.com/ruwanfer)

**Project Link:** https://github.com/ruwanfer/tuas-path-finder

---

##  Acknowledgments

- **TUAS ICT Teachers** - For curriculum guidance
- **Senior Students** - For validating path weightings
- **Classmates** - For testing and feedback

---

**Happy path finding! 🎓 May you find the perfect specialization for your future career!**
