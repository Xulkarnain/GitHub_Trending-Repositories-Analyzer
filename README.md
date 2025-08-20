#  GitHub Trending Repositories Analyzer  

This project **scrapes data from GitHub’s trending page**, stores it in a **SQLite database**, and performs analysis to identify insights such as:  
- Most starred repositories  
- Most consistent repositories in the past 7 days  
- Trends in popularity across projects  

The workflow includes **data scraping → storing → cleaning → feature engineering → visualization** for better understanding of GitHub’s trending repositories.  

---

## 🔧 Tools & Technologies  

- **BeautifulSoup4** → Web scraping GitHub trending page  
- **Requests** → Sending HTTP requests  
- **SQLite** → Local database storage  
- **Pandas** → Data cleaning & feature engineering  
- **Matplotlib** → Data visualization  
- **PyYAML** → Configuration management  
- **tqdm** → Progress bars for tracking execution  

---

## 📂 Project Workflow  

1. **Scraping**  
   - Extracts repository name and stars from GitHub Trending.  

2. **Storage**  
   - Saves the data in a **SQLite database** with schema enforcing unique `(date, repo_name)`.  

3. **Analysis**  
   - Data cleaning and feature engineering with **Pandas**.  
   - Identify **top repositories in the last 7 days**.  
   - Detect **most consistent repositories** over time.  

4. **Visualization**  
   - Plots trends (e.g., top repos by stars) for better understanding.  

---

## ▶️ How to Use  

1. **Create & Activate Conda Environment**  
   ```bash
   conda create -n github_star_repo python=3.10 -y
   conda activate github_star_repo
