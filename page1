import java.util.Scanner;

public class StudySkillsRecommendation {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.println("Welcome to the Study Skills Recommendation Program!");
        System.out.println("Let's evaluate your studying skills and provide recommendations to improve.");

        int[] scores = new int[10];
        String[] questions = {
            "How well do you manage your time when studying? (1-10)",
            "How effective are your note-taking skills? (1-10)",
            "How well do you understand and comprehend the material? (1-10)",
            "How often do you review and revise your notes? (1-10)",
            "How well do you stay focused and avoid distractions? (1-10)",
            "How comfortable are you asking questions when you don't understand something? (1-10)",
            "How frequently do you take breaks during studying? (1-10)",
            "How organized is your study space? (1-10)",
            "How well do you prepare for exams? (1-10)",
            "How confident are you in your overall study skills? (1-10)"
        };

        // Get user's scores for each question
        for (int i = 0; i < questions.length; i++) {
            System.out.print(questions[i] + " ");
            scores[i] = scanner.nextInt();
        }

        // Calculate the average score
        double averageScore = calculateAverageScore(scores);

        // Provide recommendations based on the average score
        System.out.println("\nBased on your responses, here are some recommendations to improve your study skills:");

        if (averageScore < 5) {
            System.out.println("- Focus on time management and create a study schedule.");
            System.out.println("- Practice active reading techniques to improve comprehension.");
            System.out.println("- Develop effective note-taking strategies.");
        } else if (averageScore < 8) {
            System.out.println("- Try using mnemonic devices to improve memory retention.");
            System.out.println("- Incorporate more frequent review sessions into your study routine.");
            System.out.println("- Find a study group or seek help from classmates when needed.");
        } else {
            System.out.println("- Keep up the good work and maintain your effective study habits.");
            System.out.println("- Consider mentoring others or sharing your study techniques.");
            System.out.println("- Stay motivated and continue to challenge yourself with new learning strategies.");
        }

        scanner.close();
    }

    public static double calculateAverageScore(int[] scores) {
        int sum = 0;
        for (int score : scores) {
            sum += score;
        }
        return (double) sum / scores.length;
    }
}
