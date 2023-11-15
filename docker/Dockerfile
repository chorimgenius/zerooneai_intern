# 기존 내용
FROM python:3.10

WORKDIR /tf/

USER 0

RUN mkdir -p /tf/submission/log  \
             /tf/submission/result \
             /tf/submission/submit_files \
             /tf/submission/submitted && \
    pip install jupyter ipykernel pandas numpy matplotlib seaborn

ENTRYPOINT ["jupyter", "notebook", "--ip=0.0.0.0", "--port=8888","--allow-root","--notebook-dir=/tf" ]
