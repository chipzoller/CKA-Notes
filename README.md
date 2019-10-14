# Certified Kubernetes Administrator (CKA) Notes
My notes on the Certified Kubernetes Administrator (CKA) exam


The following are some of my notes of suggestions on preparing to take the CKA exam.

### Primary Resources

- [Kubernetes in Action (Lukša)](https://www.manning.com/books/kubernetes-in-action)
  
    This is hands down the best book on the market as of this writing as it is extremely comprehensive, thorough, and very well edited. Yes, it's a little more pricey (and longer) than others, but it's of higher quality as well. The author has done a tremendous job of laying out Kubernetes from start to finish in a very logical and easy-to-digest way. The diagrams are simple and easy to follow. And there are many, many code examples that you should plan to complete (code archive freely available on GitHub). If there's only one book on Kubernetes you buy, this should be it. You should plan on not only reading this book slowly but reading each chapter twice. This is a slow process so don't rush. If you're speed reading through it without doing the examples, don't. It will take patience to absorb this information, and it's best to do so by taking your time. You will retain much more.

- [Kubeadm](https://kubernetes.io/docs/setup/production-environment/tools/kubeadm/install-kubeadm/)

    You should be extremely familiar with `kubeadm` and how to use it to provision, scale, and upgrade K8s clusters. As of the 1.16 exam, this is now an objective. Further to this, you should also be familiar with how and where `kubeadm` provisions components and configures them out-of-the-box. This is also the best environment on which to learn about Kubernetes. Things like `kind`, Minikube, and Docker Desktop are great to quickly build clusters, they are all non-standard ways to give you a cluster. Same thing goes for PaaS or prescriptive turnkey solutions like VMware PKS and OpenStack. Many of the objectives on the exam assume your cluster was provisioned with `kubeadm`, so better get very comfortable with it.

- [David-VTUK/CKA-StudyGuide](https://github.com/David-VTUK/CKA-StudyGuide)

    David has put together a great set of exam-style questions in his repo, and it comes with a solutions guide. You should go through each and every module to ensure you can perform these tasks.

- [Kubernetes the Hard Way](https://github.com/kelseyhightower/kubernetes-the-hard-way)

    Yes, you've probably been told you should know this. I would agree. However, you shouldn't need to concern yourself with going through this 20 times and memorizing every step and command by heart. Manually provisioning a K8s cluster is a great way to learn about its internals, but for the purposes of the CKA it isn't necessary. The focus of this exam is testing your practical knowledge of using K8s from a platform perspective, not building it from scratch. That said, I would recommend going through Hightower's tutorial at least twice. See my notes on a high-level overview of what the objectives are [here](https://github.com/chipzoller/CKA-Notes/blob/master/KTHW-Summarization).

- [Certified Kubernetes Administrator (CKA) with Practice Tests (Mannambeth)](https://www.udemy.com/course/certified-kubernetes-administrator-with-practice-tests/)

    The author of this course has done a pretty good job of the video lectures with nice graphics and transitions, but the real value (especially if you've already read _Kubernetes in Action_) is in the practice tests. The questions in the last two practice tests are very similar to those asked on the CKA and are hosted on Katakoda, which gives you an in-browser terminal session like the real thing.


- [Official Documentation](https://kubernetes.io/docs/home/)

    I'm sure you're tired of hearing "RTFM" but you need to do it. Most important from the documentation website are the [Tasks](https://kubernetes.io/docs/tasks/) sections. You should plan on doing most of these in your lab, but not all. At the very, very least, you should read ALL of them and know what they consist of. This will help you if you run across a scenario on the exam by knowing exactly where to go.


### Miscellaneous Tips

- Hone your Linux sysadmin skills

    This exam is 100% hands-on at a Linux command prompt and is timed. You should be more than just familiar with basic tools like `cat`, `grep`, `vim`, `ls`, `systemctl`, etc., you should be proficient. Especially when it comes to `vim`, learn how to use the proper keyboard shortcuts to navigate and manipulate text. It can be a huge time saver and also eliminate manual typing errors.

- Learn [JSONPath Expressions](https://kubernetes.io/docs/reference/kubectl/jsonpath/)

    You almost certainly will be tested on being able to either produce very specific output on the terminal or writing it out to file given some objective, and usually the request is targeting [JSONPath expressions](https://kubernetes.io/docs/reference/kubectl/jsonpath/). Spend time to become very familiar and comfortable with it, including the various functions.

- Manage time
  
    You have 3 hours to complete 24 questions. Some questions will take you less than a minute, others will take you possibly 10 minutes. In my experience, I found the time more than generous, but if you get in there and are discovering every question is taking more than than the 7.5 minutes you have on average to complete them, you aren't prepared enough. Keep in mind, the purchase of your exam comes with one free retake, and you don't get a partial refund if you pass on the first attempt. If you find you aren't well enough prepared on your first attempt, do not worry, but use the time to peruse all the questions and take mental note of where your gaps are. Once you've ended the exam, immediately write them down and begin to pound on them during your next lab session.

- Follow Directions
  
    This might be trite, but I can't be more serious. You need to read the damn directions multiple times before you touch the keyboard. And when you think you've successfully completed the question, you need to read them **once again and verify, slowly and carefully**, that you've done it exactly as written. This exam is proctored by a live human but scored by statistical sampling, so if the question asked you to create a Pod with the name of `nginx` and you created it with the name of `web` or even `nginz`, you're likely not getting points for your attempt even though it may be effectively correct.

- Be Calm, Type Slowly

    24 questions in 180 minutes should be plenty of time if you know what you're doing, so be calm (however you accomplish that) and type slowly. Read the bullet above about how the test is scored. If you're making typos because you're trying to speed through it, you will likely receive no points for that question. It behooves you to think calmly and type slowly.
