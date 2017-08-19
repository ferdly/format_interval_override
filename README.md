# format_interval_override
Drupa Ago (format_interval) actually accurate

Raison Detre
The 'ago' function supplied by Drupal is not accurate. Really?
* see example ('get_date_array(2);//Wrong! Just before my birthday...')
I intend to write a better one. Based on a few days before my birthday from my birthdate this example fails.

I believe that I can do better, without too much pain. This method is based on these two premises:

* The mod($inteval, $seconds_in_1day) is always the correct number of $seconds for constructing the time
* The floor($iterval/$seconds_in_1day) is always the correct number of $days for constructing the date

Thus the work is getting accurate years months, weeks and days from this

http://phptester.net
