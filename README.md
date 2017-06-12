# QRontol
Control stuff via QR codes, that trigger python scripts.

The main idea is to provide a tangible interface to control user-defined actions, e.g., as an alternative to a touch screen interface. The inspiration comes from the "old way" of browsing for music, e.g., by flipping through some LP or CD albums covers in a box. So one of the use cases is to create/print album QR cards, e.g., having a set of cards with QR codes on them. Then one can browse through the deck of cards and pick an album, scan it which triggers an action that starts the playlist on a streaming music service or starts the album in a local mp3 player etc. 

# System overview
* printed QR code tags
* QR code reader which either is a
 * custom reader: interprets the code and triggers a command or
 * generic reader: visits a special URL, that triggers a command elsewhere
* command server: receives command and triggers a command/action at any third party API
