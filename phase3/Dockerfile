FROM drupal:8.8

RUN apt-get update && apt-get install -y git \
    && rm -rf /var/lib/apt/lists/*

WORKDIR /var/www/html/themes

RUN git clone --branch 8.x-3.24 --single-branch --depth 1 https://git.drupal.org/project/bootstrap.git \
  && chown -R www-data:www-data bootstrap
