FROM php:5.6.4-apache
RUN apt-get update && apt-get install -y \
  vim \
  less
RUN ln -sf /usr/share/zoneinfo/Asia/Tokyo /etc/localtime
RUN mkdir -p /root/.vim/colors
COPY ./php.ini /usr/local/etc/php/
COPY ./dotfiles/vimrc /root/.vimrc
COPY ./dotfiles/jellybeans.vim /root/.vim/colors
COPY ./dotfiles/bashrc /root/.bashrc
