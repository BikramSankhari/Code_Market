FROM python:3.11.4-alpine

WORKDIR /usr/src/app

# prevent Python from writing .pyc files
ENV PYTHONDONTWRITEBYTECODE=1
# ensure Python output is sent directly to the terminal without buffering
ENV PYTHONUNBUFFERED=1
ENV SECRET_KEY=a_Sup€¤_&€creT)Key2Crr@@@ccKKBYE@n!u$€¤


RUN pip install --upgrade pip
COPY Code_Market/ Code_Market/
COPY Django_Img/ Django_Img/
RUN pip install -r Code_Market/requirements.txt

ENTRYPOINT ["./Django_Img/entrypoint.sh"]