FROM adnrv/texlive:basic

# Minted + Pygments
RUN tlmgr option repository http://mirror.ctan.org/systems/texlive/tlnet && \
    tlmgr update --self && \
    tlmgr install chktex babel-polish gustlib memoir ebgaramond xkeyval fontaxes tex-gyre listings xpatch etoolbox layouts printlen enumitem datetime fmtcount

RUN apt update && apt install -y \
    git \
    && rm -rf /var/lib/apt/lists/*