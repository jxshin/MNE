This is the dataset of the paper "An Empirical Study of Multiple Names and Email Addresses in OSS Version Control Repositories".

The sampled repositories are listed in the file "sampled_repositories.txt",
where each line is a repository, the fields are separated by ";",
the first filed indicates the group the repository belong to, and the second field is the full name of the repository.

The commit logs of all the repositories are stored in the file "commit_logs_all_repos.zip".
where each line is a commit, and the schema is:
repo_full_name;commit_id;committer_name;committer_email;commit_time;author_name;author_email;author_time

The merged names and emails are listed in the file "all_developers_merged_masked.txt",
where each line is a developer, names and email addresses are separated by "|-:+|",
names are separated by "|-;+|", and email addresses are separated by |-;+|.
**Note: The postfixes of the email addresses are masked by MD5 for developers' privacy.
The MD5 is calculated through hashlib.md5 in Python.**

You can use the file "commit_logs_all_repos.zip" to get the file "all_developers_merged_masked.txt".
You can use the file "sampled_repositories.txt", "commit_logs_all_repos.zip" and "all_developers_merged_masked.txt"
to get all the results presented in the paper.
Be careful of the encoding of the files in the process.
