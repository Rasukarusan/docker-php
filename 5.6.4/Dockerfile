FROM php:5.6.4-apache
RUN apt-get update && apt-get install -y \
  vim \
  less \
  # php-extentionsを入れるために必要なパッケージ
  libfreetype6-dev \
  libjpeg62-turbo-dev \
  libmcrypt-dev \
  libpng-dev \
  libgmp-dev
RUN ln -s /usr/include/x86_64-linux-gnu/gmp.h /usr/include/gmp.h

RUN docker-php-ext-install mcrypt gmp gettext mbstring sockets sysvsem sysvshm
RUN ln -sf /usr/share/zoneinfo/Asia/Tokyo /etc/localtime
RUN mkdir -p /root/.vim/colors
COPY ./php.ini /usr/local/etc/php/
COPY ./dotfiles/vimrc /root/.vimrc
COPY ./dotfiles/jellybeans.vim /root/.vim/colors
COPY ./dotfiles/bashrc /root/.bashrc
