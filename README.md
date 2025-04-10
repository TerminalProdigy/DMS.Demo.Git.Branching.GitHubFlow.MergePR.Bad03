# DMS.Demo.Git.Branching.GitHubFlow.MergePR.Bad03
Steps taken to replicate:
1. Create a new class library project.
2. Add project to source control.
3. Create feature branch named 'feature/foo' & checkout.
4. Add a new class named 'Class2.cs'.
5. Add a comment to 'Class2.cs' : '// Branch: feature/foo | Commit #1'.
6. Commit changes: 'Branch: feature/foo | Commit #1'.
7. Checkout 'master' branch.
8. Add a comment to 'Class1.cs' : '// Branch: master | Commit #2'
9. Commit changes: 'Branch: master | Commit #2'.
10. Checkout branch 'feature/foo'.
11. Merge branch 'master' into 'feature/foo'.
12. Add a comment to 'Class2.cs' : '// Branch: feature/foo | Commit #3'
13. Commit changes: 'Branch: feature/foo | Commit #3'.
11. Add a comment to 'Class2.cs' : '// Branch: feature/foo | Commit #4'
12. Commit changes: 'Branch: feature/foo | Commit #4'.
13. Create a PR branch from 'feature/foo' named 'pull/2/merge' & checkout.
15. Push branches 'master' & 'pull/2/merge'.
16. Create a new pull request. Merge Into: 'master' | From: 'pull/2/merge'
17. Merge pull request.
18. Checkout branch 'master'.
19. Pull latest changes.
20. Evaluate commit history/line.

![image](https://github.com/user-attachments/assets/4f76b103-c5bf-471a-8125-89c2bc60a6bd)