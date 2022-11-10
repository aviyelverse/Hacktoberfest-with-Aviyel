Link to the Article => https://aviyel.com/post/3857/

## Introduction to Novu❗

[Novu](https://novu.co/) is an open source notification infrastructure for developers. It simply requires simple components and APIs for managing all communication channels like email, SMS, chat, and push. We can use novu to send notifications in just three simple steps:

1. **Create template**
2. **Connect Integrations**
3. **Trigger to notify**

Currently, it supports both [self-hosted](https://docs.novu.co/overview/docker-deploy/) (local) and [cloud-based](https://web.novu.co/templates) notification services. However, because this blog is only about Novu Web Studio, we will concentrate on cloud-based notification services.

## Web Studio Walkthrough🚶🏼

Initially, head to the [web dashboard](https://web.novu.co/templates) and sign up either using GitHub or email. Further steps assume that you are signed into the web dashboard. Do save your changes when and where necessary to avoid losing progress.

Different steps involved to create notifications in Web Studio are:


![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/kqrov9zhngyxdg1e6iw8.png)



### 1). Head to the Integrations store:

On the [integration store](https://web.novu.co/integrations), you can find a list of available integrations organized into categories like:

- Email
- SMS
- Chat
- Push
    

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/9gpqf74diufqkok60a2y.png)



All of them perform respective actions of sending email, SMS, and push notifications. To add a new integration, click on the `Connect` button below the respective integration and fill in the credentials acquired from the respective platform. Each integration requires different details, so make sure to be careful while filling in the details.

### 2) Go to Notification Template:

Let's create a new [notification template](https://web.novu.co/templates) by hitting the `New` button. Then we have to fill in the required details like:

- Notification Name
- Notification Description
- Notification Identifier
- Notification Group


![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/axdut1qrsfehygf22kno.png)



> Note: Eyes wide while filling in the Identifier as it will be used further.
> 

After filling in the details, if you hit `Create` , then you will be able to find the Trigger implementation code. It looks similar to this:


```
import { Novu } from '@novu/node';
const novu = new Novu('<API_KEY>');
novu.trigger('test-01', {
  to: {
    subscriberId: '<REPLACE_WITH_DATA>'
  },
  payload: {
  }
});
```

### 3) Create a Workflow:


![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/19npcbapwrizflrg9mif.png)



This is the workflow of what has to happen when triggered from our application. Let’s focus on sending emails to the subscribers. To begin, simply click on the ➕ icon and select email. However, once you are done with it, you will notice a red dot(🛑). If you click `Edit Template`, you will be prompted to enter an email subject and body. Use your own content and then click `Update`.

🎉Hurrah! You have successfully configured your web studio to send notifications when triggered. The next step is to use the code generated from the `Trigger Snippet` in your application. Let’s see other features that are available and provided by novu.

### 4) Special Features

- Also, you can [collaborate](https://web.novu.co/team) while working on the app with the team members.
    
    
![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/o690xeo1mwkqwejx7f6q.png)


    
- Use your specific [brand](https://web.novu.co/settings) logos and themes to make your notification unique.
    
    
![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/c6ggqbqlthqjjypq2wiq.png)


    
- Take a look at the [Activity Feed](https://web.novu.co/activities) to see the notification trigger details in a graphical view.
    
    
![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/3xxrhdhqtoz9m1uvdomm.png)


## Conclusion

We have covered a lot of ground here, but there is plenty more to explore and experiment with within the realm of this free and open source notification infrastructure tool. Please feel free to take a look at the [documentation](https://docs.novu.co/), which will give you an understanding of anything that is hindering your progress. Join the [discord](https://discord.com/invite/9wcGSf22PM) and [contribute](https://github.com/novuhq/novu) to its open issues, bugs, or features—whatever interests you about Novu!
