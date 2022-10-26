# 👨‍💻️ CV Arjen Bos
Voor het ontwerp van mijn CV gebruik ik HTML en CSS met [Tailwind](https://tailwindcss.com). En met Python en [Jinja](https://jinja.palletsprojects.com/) laad ik de data, zoals de projecten die ik uitgevoerd heb, in de templates.

Hier zijn de instructies om deze repo te klonen en het CV te renderen.

### Eenmalige setup (in terminal)
1) Clone deze repo `git clone https://github.com/arjobsen/bosconsultant.nl`
1) Navigeer naar deze folder `cd bosconsultant.nl`
1) Maak een Python virtual environment `python3 -m venv venv`
1) Activeer de venv, zie eventueel de [docs](https://docs.python.org/3/library/venv.html) welk commando geschikt is voor jouw computer
    * Op Windows met cmd gebruik `venv\Scripts\activate.bat`
    * Op Linux met fish gebruik `source venv/bin/activate.fish`
1) Check eventueel met `which python` (Linux) of `python` nu daadwerkelijk verwijst naar de zojuist aangemaakte venv
1) Installeer de vereiste packages in de venv `pip install -r requirements.txt`

### Templates met data render naar index.html
Ik gebruik Python en [Jinja](https://jinja.palletsprojects.com/) om data, een yaml met de projecten, dynamisch in mijn CV te laden.
1) Activeer de venv mocht die nog niet geactiveerd zijn
1) Navigeer naar de cv folder `cd cv`
1) Run `python render.py`
