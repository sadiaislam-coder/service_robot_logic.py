# Project: Human-Robot Interaction (HRI) Logic
# Focus: How a service robot responds to customer feedback

def robot_interaction_system():
    print("--- Service Robot: Customer Feedback System ---")
    print("Robot: Hello! How was your experience with our service today?")
    
  # Taking simple text feedback
  feedback = input("Customer: ").lower()

  # Business Keywords for Sentiment Analysis
   positive_words = ["good", "great", "happy", "excellent", "fast"]
    negative_words = ["bad", "slow", "angry", "expensive", "poor"]

   print("\n[Robot is processing your feedback...]")

   # Logic: Checking words in the feedback
   if any(word in feedback for word in positive_words):
        action = "Robot Action: Perform a happy 'Thank You' dance and offer a discount coupon! 💃"
        strategy = "Marketing Strategy: Reward the loyal customer."
    elif any(word in feedback for word in negative_words):
        action = "Robot Action: Bow down and notify the human manager immediately. 🙇‍♂️"
        strategy = "Marketing Strategy: Crisis management and retention."
    else:
        action = "Robot Action: Give a polite nod and say 'Thank you for your feedback!'"
        strategy = "Marketing Strategy: Standard engagement."

   # Final Output
   print(f"Result  : {action}")
  print(f"Insight : {strategy}")
  print("--- System Standby ---")

if __name__ == "__main__":
    robot_interaction_system()

