// function to send message to Slack
function sendToSlack() {
  var timestamp = new Date();
   var student= ["#abhay-test-automate", "Volvo", "BMW", "kaka", "mama", "dada", "ata", "tata", "papa", "papaa", "phupha", "bua"];
  // custom slack webhook
  // change the XXXXX's to your own slack webhook. Get it from: 
  // https://my.slack.com/services/new/incoming-webhook/
  var url = "https://hooks.slack.com/services/YYYYYYYYYYYY/ZZZZZZZZ/XXXXXXXXXXXXXXXXXXXXXXXX";
   
  var payload = {
    "channel": "#abhay-test-automate",
    "username": "abhey101",
    "text": "Hi " + student[2] +
      "\n Here are your project scores and feedack. Let us know if you have any questions! \n" +
      "\n Section 1 Score: " + student[5] +
      "\n Section 2 Score: " + student[6] +
      "\n Section 3 Score: " + student[7] +
      "\n Overall Score: " + student[8] +
      "\n *Positive notes:* " + student[9] +
      "\n *Areas for improvement:* " + student[10] +
      "\n *Any other comments:* " + student[11] +
      "\n \n Marked by: " + student[3] +
      "\n Date: " + timestamp +
      "\n \n Sent care of Marking Mail Merge tool built.",
    "icon_emoji": ":inbox_tray:"
  };
 
  var options = {
    "method": "post",
    "contentType": "application/json",
    "payload": JSON.stringify(payload)
  };
   
  return UrlFetchApp.fetch(url,options);
}
