### These are the notes of the developer Ryan Miller for the Fly.io coding sample:

### Changes

live/app_live/show.ex
- added deployment_status field to the socket to be accessed in the view (see line 14)
- added deployment_status_id because I thought this would be the ID needed to access the deployment status in graphQL. I am wrong about this apparently (see line 15, 25-26, 43-44)
- added private function called get_template_deployment_status 


lib/client/client.ex
- added some fields to access allocations data from graphQl
- added broadcast fields to enable LiveView reload (line 124, 230, 341, 343-346)

lib/fly_web/live/app_live/show.html.heex
- added fields for instances. A very basic implementation (line 154-249)
- added fields for deployment status info (see comment on line 52)

### what I built
- Made changes to graphQL requests to pull in more data
- altered views to show the data
- added broadcast features to the page

### what I didn't build
- Tests! I'd love to learn how to test LiveView properly 
- Really solid UI. There is a CSS issue with the instance data rendering which I did not take the time to fix. It looks a little janky, but gets the job done showing I can get the data to the page

### how I'd determine the feature is successful
- tests! I can write rspec tests but it seemed it might take too long to learn an elixir testing framework. Happy to learn this weekend though!

### Other notes about the assessment 

Having never looked at Elixir/Phoenix before a week ago, I think I have a good grasp of the application. I really enjoyed working on this! Unfortunately the issues with  accessing the deployment_status id from graphQL stood in my way to acheive a completely finished product. Next steps for this app would definitely be implementing tests to ensure LiveView is updating exactly how I want it to 


### other 
I am really interested in working at Fly.io . I enjoyed my conversation with Michael and think I could be a great addition to the team. I enjoy learning lots of different technologies and thinking outside the box (my greatest strength is coming up with solid ideas on the spot). I'd be really excited to work here and would work hard to become a senior engineer in no time :)