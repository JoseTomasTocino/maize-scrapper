Instruction.

1. Create virtualenv:
virtualenv -p /usr/bin/python3 street-food-scraper

2. Activate:
cd street-food-scraper && source bin/activate

3. Clone project:
git clone https://github.com/kirimaks/street-food-scraper.git && cd street-food-scraper

4. Install requirements:
# On Ubuntu/Debian: sudo apt install python-dev libssl-dev libxml2-dev libxslt1-dev liblzma-dev
pip install -r requirements.txt

5. Run scraper:
cd street_food 
scrapy crawl get-food-yelp -o yelp-data.csv                 # Get data from yelp.com
scrapy crawl get-food-offthegrid -o offthegrid-data.csv     # Get data from offthegrid.com
