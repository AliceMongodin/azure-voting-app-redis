FROM tiangolo/uwsgi-nginx-flask:python3.6
RUN pip install redis
ADD /azure-vote /app

HEALTHCHECK --interval=1m --timeout=30s --retries=3 CMD curl --fail http://localhost:80 || exit 1