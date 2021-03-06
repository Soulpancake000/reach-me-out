<p align="center">
  <img src="https://user-images.githubusercontent.com/37014061/87138394-a3fb5400-c29e-11ea-862b-8fd43a3f44e6.JPG" alt="app-logo"/>
  <p align="center">ServiceNow Application allow administrators to add social links feature to the user reference fields on form level.</p>
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/37014061/87136513-e7a08e80-c29b-11ea-9d25-ac6f7ba1794f.JPG" alt="app-form"/>
</p>

**On User Configurations Table Form:** 
<ul>
  <li><b>Active:</b> Only active records would be considerable</li>
  <li><b>User:</b> Ref field to user oob sys_user table</li>
  <li><b>Social Link:</b> Valid link corresponded to the social network choice</li>
  <li><b>Social Network:</b> Custom choice list determine social network icon that would be displayed on target form</li>
  
  <li><b>Table:</b> Target table</li>
  <li><b>Target Ref:</b> filtred list contain user-ref fields type from the selected table</li>
</ul>

**Output:** 
 <p align="center">
  <img src="https://user-images.githubusercontent.com/37014061/87136919-73b2b600-c29c-11ea-9b78-b370b91df3e8.JPG" alt="app-result"/>
 </p>

**Troubleshooting:**
 <p align="left">
   In case of <b>..cross-scope access policy</b> issue, please set the client script table <b>sys_script_client</b> accessibility to <b>All application scope</b> with <b>Can create & Can update</b> privileges as described in this article: https://hi.service-now.com/kb_view.do?sysparm_article=KB0727180
  </p>

# Generated files
This repository contains generated files and a checksum.

**Do not edit the files in this repository outside of an instance of ServiceNow.**

If you find yourself unable to import your repository due to the presence of files edited outside an instance of ServiceNow, merge commits that mix files from different revisions, or other data that does not match the checksum, you may recover using either of the following techniques:
* Remove the problem commits:
  1. Clone your repository to a personal computer with the git command line tools installed and open a git command prompt in the repository root
  2. Run `git log` and take note of the SHA1s of the problem commits
  3. Build revert commits using `git revert SHA1` repeatedly, working backward in time, for each commit that introduced changes not generated by a ServiceNow instance
  4. Run `git push`

* Overwrite the problem code snapshot with a known good one:
  1. Clone your repository to a personal computer with the git command line tools installed and open a git command prompt in the repository root,
  2. Locate a known good code snapshot and record its SHA1. For this step, `git log` can be useful.
  2. Run `git reset --hard SHA1` to a commit that was generated by a ServiceNow instance
  3. Run `git reset HEAD{1}`
  4. Run `git add -A`
  5. Run `git commit`
  6. Run `git push`
