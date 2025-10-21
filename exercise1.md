Most important thing is linter/formatter for the project to guarantee same syntax and easy readability. For python the linter/formatter would be ruff, it seems to be the most used.  
For testing Python has playwright/pytest. I would steer much more towards e2e as those can test the site in it's totality.  
Pretty sure building for python is just pip.  
Alternatives for ci are plenty like circle, gitlab, azure, though I don't see much reason to not just use github, especially if you're already used to it.  
I would like to self host at least ci because the tests take a while on free cloud machines. Playwright specifically takes a while with the installations, but I think it is still worth it. The pricing for paid cloud machines seems extremely steep and frankly looks like robbery for people who are stuck in their ecosystems and want more compute. The only plus seems to be instant scalability and ease of use, but especially for effectively hobbyist level, where you already have spare compute on your pc, cloud doesn't make much sense.  
For the non compute heavy portions like hosting the actual git etc, self hosting doesn't seem too important. Though backups would be preferable.
