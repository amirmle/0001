# 0001
6521510069:AAGnFG8nHudkvjgAD77ZgFANYaaBrLkIaT8  
curl -s "https://api.telegram.org/bot$OS_TOKEN/getUpdates" | jq -r '.result[0].message.chat.id  

curl -s -X POST -H 'Content-Type: application/json' -d "{\"chat_id\": $OS_ID, \"text\": \"User login detected:\n$OS_DATE\n$OS_HOSTNAME\n$OS_IP\n$USER\", \"disable_notification\": false}" "https://api.telegram.org/bot$OS_TOKEN/sendMessage"  > /dev/null 2>&1

