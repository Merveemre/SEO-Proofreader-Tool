## SEO Proofreader Tool

Python-based automated SEO analysis tool prototype that scores content pages against checklists and provides actionable optimization recommendations.

### Requirements
- Python 3.7+ (programming language and runtime environment)
**Python Packages:**
- pandas>=1.5.0 (for data manipulation and CSV file handling)
- jupyter>=1.0.0 (for running the .ipynb notebook file)

**Installation:**
```bash
pip install pandas jupyter
```

### How to Run
Download the project
Start Jupyter Notebook
Run the analysis:
- Open `codes.ipynb` 
- Click "Run All" 
- The tool will analyze all sample articles automatically

**Check results:**
- Analysis reports will be generated as .txt files in the main folder
- Each report shows scores and specific recommendations

### What This Tool Does
This tool automatically checks SEO content against official guidelines and gives scores out of 100 points:

**Content Analysis Features:**
- **Page Titles:** Checks length, keywords, and formatting
- **Meta Descriptions:** Validates content and call-to-actions  
- **Keywords:** Measures keyword density (optimal: 0.5%-2.5%)
- **Internal Links:** Finds links to relevant pages
- **Formatting:** Validates price formats (€ 1.200,-) and percentages (30%)
- **Content Quality:** Checks paragraph length and readability

**What You Get:**
- Detailed score breakdown for each content category
- Specific recommendations for improvement
- Pass/fail indicators for each SEO rule
- Summary reports saved as text files

### Sample Results
The tool has been tested on 4 different articles:
- Cost page: Thuisbatterij (battery costs)
- Cost page: Schutting (fence costs)  
- City page: Elektricien Haarlem (electrician in Haarlem)
- City page: Relatietherapie Amsterdam (relationship therapy in Amsterdam)

Each analysis takes seconds instead of the usual 1-hour manual process.

### Technical Details
- Built with Python 3 using standard libraries
- Lightweight approach: Uses regex and pandas instead of heavy NLP libraries
- Fast processing: Analyzes articles in seconds
- Easy to modify: All analysis rules are clearly defined in the code

### Limitations
**Input Format:**
- Text file dependency: Only works with .txt files, not Word documents or HTML
- Prefix requirement: Needs "title:" and "meta:" prefixes in input files
- Missing data impact: City pages scored lower because they lacked proper formatting

**Analysis Scope:**
- Simple page type detection based on keywords
- No grammar/spelling checks (coming in future versions)
- CSV conversion required: Original Excel files needed manual conversion to CSV format

## Future Improvements
- Web interface using Flask for easier use
- Grammar checking with advanced language tools
- Better document parsing for Word/HTML files
- More detailed scoring with SEO team input
