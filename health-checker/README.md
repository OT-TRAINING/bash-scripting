WAP that will do the health check of all added  URL at every Health Check duration   and send the slack/mail notification if it unhealty 

./healthChecker  add -u <url> -d <duration> [-e <email>] [-s <slack channel>]
./healthChecker  update -u <url> -d <duration> [-e <email>] [-s <slack channel>]
./healthChecker  remove -u <url>
./healthChecker  list
./healthChecker  add -u www.opstree.com -d 30m  -s ot-health-check
./healthChecker  update -u www.opstree.com -d 1h -s ot-health-check
