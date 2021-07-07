# legendary-octo-disco-88
ctx.logger.debug('debug info'); ctx.octo.info('some request data: %j', ctx.request.body); ctx.logger.warn('WARNNING!!!!');
legendary-octo-disco
NPM version build status Test coverage David deps Known Vulnerabilities npm download

Sentry SDK for Octo-Disco

Install
$ npm i octo-logger-sentry --save
Configuration
Change ${app_root}/config/plugin.js to enable octo-logger-sentry plugin:

exports.loggerSentry = {
  enable: true,
  package: 'Octo-logger-sentry',
};
Configure information in ${app_root}/config/config.default.js:

exports.loggerSentry = {
  dsn: 'https://<hash>@example.com/<id>'
};
see config/config.default.js for more detail.

Usage
ctx.logger.debug('debug info');
ctx.logger.info('some request data: %j', ctx.request.body);
ctx.logger.warn('WARNNING!!!!');
Questions & Suggestions
Please open an issue here.

License
MIT
