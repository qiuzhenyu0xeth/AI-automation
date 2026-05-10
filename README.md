# AI Automation Task Checker

tasks = {
    "Collect data": False,
    "Analyze data": False,
    "Generate summary": False,
    "Send notification": False
}

def automate(task_dict):
    print("AI automation started...\n")

    for task in task_dict:
        task_dict[task] = True
        print(f"{task} completed")

    print("\nFinal status:")
    for task, done in task_dict.items():
        print(f"{task}: {'Done' if done else 'Pending'}")

if __name__ == "__main__":
    automate(tasks)
