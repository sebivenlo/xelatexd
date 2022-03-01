FROM aergus/latex:latest
USER latex
RUN mkdir -p /home/latex/wd
COPY rcmd scmd quit /usr/local/bin/
CMD /usr/local/bin/rcmd
