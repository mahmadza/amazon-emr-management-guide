# Add a Git Repository to Amazon EMR<a name="emr-git-repo-add"></a>

**To add a Git repository as a resource in your Amazon EMR account**

1. Open the Amazon EMR console at [https://console.aws.amazon.com/elasticmapreduce/](https://console.aws.amazon.com/elasticmapreduce/)\.

1. Choose **Git repositories**, then choose **Add repository**\.

1. For **Repository name**, enter a name to use for the repository in Amazon EMR\. 

   Names may only contain alphanumeric characters, hyphens \(\-\), or underscores \(\_\)\.

1. For **Git repository URL**, enter the URL for the repository\.

1. For **Branch**, enter a branch name\. 

1. For **Git credentials**, choose the credentials to use to authenticate to the repository\.
   + Choose **Use an existing AWS secret** and select a secret from the list\.

     The existing secret must be in the following format: \{"gitUsername": UserName, "gitPassword": Password\}\.
   + Choose **Create a new secret**\. 
     + If you use **Username and password**, enter a name for the secret, and then enter the username and password\.
     + If you have two\-factor authentication enabled for your Git repository, choose **Personal access token \(PAT\)**\. We recommend using a personal access token generated by your Git service provider instead of your account password\. For more information, see [Creating a personal access token for the command line for GitHub](https://help.github.com/articles/creating-a-personal-access-token-for-the-command-line/) and [Personal access tokens for Bitbucket](https://confluence.atlassian.com/bitbucketserver/personal-access-tokens-939515499.html)\.
   + Choose **Use a public repository without credentials** if the Git repository is public\.

1. Choose **Add repository**\. 