{
  "name": "MindSparked Setup",
  "description": "Initial Pinokio automation: tests GitHub connection and sets up local MindSparked folder structure.",
  "version": "1.0.0",
  "run": [
    {
      "method": "shell.run",
      "params": {
        "command": "mkdir \"C:\\Leo\\MindSparked\" && mkdir \"C:\\Leo\\MindSparked\\github-test\""
      }
    },
    {
      "method": "git.clone",
      "params": {
        "repo": "https://github.com/octocat/Hello-World",
        "target": "C:\\Leo\\MindSparked\\github-test"
      }
    },
    {
      "method": "shell.run",
      "params": {
        "command": "echo MindSparked Pinokio setup complete! > \"C:\\Leo\\MindSparked\\SETUP_SUCCESS.txt\""
      }
    }
  ]
}
