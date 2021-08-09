# Hata-AntiCheat

Eklentiyi kullanmadan önce modun boş bir yerine bu kodları ekleyin;

public OnPlayerCheatDetected(playerid, code)
{
    new cheatname[128], string[128];
    switch (code)
    {
        case 0: cheatname = "Silent Aimbot";
        case 1: cheatname = "Vehicle Repair Hack";
        case 2: cheatname = "Screen Flickering";
        case 3: cheatname = "Car Troller";
        case 4: cheatname = "Surfing Invisible";
        case 5: cheatname = "Airbreak";
        case 6: cheatname = "Seat Crasher";
        case 7: cheatname = "Speed Hack";
        case 8: cheatname = "Troll Animation";
        case 9: cheatname = "Animation Invisible";
        case 10: cheatname = "Fly Hack";
        case 11: cheatname = "Rage Shot";
        case 12: cheatname = "Trailer Crasher";
        case 13: cheatname = "Weapon Hack";
        case 14: cheatname = "Kill All";
        case 15: cheatname = "Checkpoint Teleport";
        case 16: cheatname = "Quick Turn";
        case 17: cheatname = "NPC Login";
        case 19: cheatname = "Game Speed";
        case 18: cheatname = "Fake State";
    }
    format(string, sizeof(string), "Hata Anti Cheat tarafından %s tespit edildi ve oyundan atıldınız.", cheatname);
    SendClientMessage(playerid, 0xA9C4E4FF, string);
    Kick(playerid);
    return 1;
}
