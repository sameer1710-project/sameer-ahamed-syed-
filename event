#include <stdio.h>
#include <string.h>

#define MAX 100

// -------- Structures --------
struct Event {
    int id;
    char name[50];
    char date[20];
    char venue[50];
};

struct Activity {
    int id;
    char title[50];
    char time[20];
    char facilitator[50];
};

// -------- Global Arrays --------
struct Event events[MAX];
struct Activity activities[MAX];
int eventCount = 0, activityCount = 0;


// -------- Add Event --------
void addEvent() {
    if (eventCount >= MAX) {
        printf("Event list full!\n");
        return;
    }

    struct Event e;
    printf("Enter Event ID: ");
    scanf("%d", &e.id);

    getchar();
    printf("Enter Event Name: ");
    fgets(e.name, 50, stdin);
    e.name[strcspn(e.name, "\n")] = '\0';

    printf("Enter Event Date: ");
    fgets(e.date, 20, stdin);
    e.date[strcspn(e.date, "\n")] = '\0';

    printf("Enter Event Venue: ");
    fgets(e.venue, 50, stdin);
    e.venue[strcspn(e.venue, "\n")] = '\0';

    events[eventCount++] = e;
    printf("Event added successfully!\n");
}


// -------- Add Activity --------
void addActivity() {
    if (activityCount >= MAX) {
        printf("Activity list full!\n");
        return;
    }

    struct Activity a;
    printf("Enter Activity ID: ");
    scanf("%d", &a.id);

    getchar();
    printf("Enter Activity Title: ");
    fgets(a.title, 50, stdin);
    a.title[strcspn(a.title, "\n")] = '\0';

    printf("Enter Activity Time: ");
    fgets(a.time, 20, stdin);
    a.time[strcspn(a.time, "\n")] = '\0';

    printf("Enter Facilitator Name: ");
    fgets(a.facilitator, 50, stdin);
    a.facilitator[strcspn(a.facilitator, "\n")] = '\0';

    activities[activityCount++] = a;
    printf("Activity added successfully!\n");
}


// -------- View Events --------
void viewEvents() {
    if (eventCount == 0) {
        printf("No events available.\n");
        return;
    }

    printf("\n--- Events List ---\n");
    for (int i = 0; i < eventCount; i++) {
        printf("ID: %d\nName: %s\nDate: %s\nVenue: %s\n\n",
               events[i].id, events[i].name, events[i].date, events[i].venue);
    }
}


// -------- View Activities --------
void viewActivities() {
    if (activityCount == 0) {
        printf("No activities available.\n");
        return;
    }

    printf("\n--- Activities List ---\n");
    for (int i = 0; i < activityCount; i++) {
        printf("ID: %d\nTitle: %s\nTime: %s\nFacilitator: %s\n\n",
               activities[i].id, activities[i].title,
               activities[i].time, activities[i].facilitator);
    }
}


// -------- Search Event by ID --------
void searchEvent() {
    int id;
    printf("Enter Event ID to search: ");
    scanf("%d", &id);

    for (int i = 0; i < eventCount; i++) {
        if (events[i].id == id) {
            printf("\nEvent Found:\nID: %d\nName: %s\nDate: %s\nVenue: %s\n",
                   events[i].id, events[i].name, events[i].date, events[i].venue);
            return;
        }
    }
    printf("Event not found.\n");
}


// -------- Search Activity by ID --------
void searchActivity() {
    int id;
    printf("Enter Activity ID to search: ");
    scanf("%d", &id);

    for (int i = 0; i < activityCount; i++) {
        if (activities[i].id == id) {
            printf("\nActivity Found:\nID: %d\nTitle: %s\nTime: %s\nFacilitator: %s\n",
                   activities[i].id, activities[i].title,
                   activities[i].time, activities[i].facilitator);
            return;
        }
    }
    printf("Activity not found.\n");
}


// -------- Delete Event --------
void deleteEvent() {
    int id;
    printf("Enter Event ID to delete: ");
    scanf("%d", &id);

    for (int i = 0; i < eventCount; i++) {
        if (events[i].id == id) {
            for (int j = i; j < eventCount - 1; j++)
                events[j] = events[j + 1];

            eventCount--;
            printf("Event deleted successfully!\n");
            return;
        }
    }
    printf("Event not found.\n");
}


// -------- Delete Activity --------
void deleteActivity() {
    int id;
    printf("Enter Activity ID to delete: ");
    scanf("%d", &id);

    for (int i = 0; i < activityCount; i++) {
        if (activities[i].id == id) {
            for (int j = i; j < activityCount - 1; j++)
                activities[j] = activities[j + 1];

            activityCount--;
            printf("Activity deleted successfully!\n");
            return;
        }
    }
    printf("Activity not found.\n");
}


// -------- Main Menu --------
int main() {
    int choice;

    while (1) {
        printf("\n==== Events / Activities Management System ====\n");
        printf("1. Add Event\n");
        printf("2. Add Activity\n");
        printf("3. View Events\n");
        printf("4. View Activities\n");
        printf("5. Search Event\n");
        printf("6. Search Activity\n");
        printf("7. Delete Event\n");
        printf("8. Delete Activity\n");
        printf("9. Exit\n");
        printf("Enter your choice: ");
        scanf("%d", &choice);

        switch (choice) {
            case 1: addEvent(); break;
            case 2: addActivity(); break;
            case 3: viewEvents(); break;
            case 4: viewActivities(); break;
            case 5: searchEvent(); break;
            case 6: searchActivity(); break;
            case 7: deleteEvent(); break;
            case 8: deleteActivity(); break;
            case 9:
                printf("Exiting program...\n");
                return 0;
            default:
                printf("Invalid choice! Try again.\n");
        }
    }
}
