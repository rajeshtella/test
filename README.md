public class Main {
    public static void main(String[] args) {
        LocalDateTime localDateTime = LocalDateTime.now(); // Get current LocalDateTime

        // Specify the timezone (ZoneId)
        ZoneId zoneId = ZoneId.of("America/New_York"); // Example: New York timezone
        ZonedDateTime zonedDateTime = localDateTime.atZone(zoneId); // Convert LocalDateTime to ZonedDateTime in specified timezone

        System.out.println("ZonedDateTime: " + zonedDateTime);
    }
}
