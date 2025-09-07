<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CaféPlan Pro - Gestão Rural Completa</title>
    
    <!-- PWA Meta Tags -->
    <meta name="theme-color" content="#047857">
    <meta name="apple-mobile-web-app-capable" content="yes">
    <meta name="apple-mobile-web-app-status-bar-style" content="default">
    <meta name="apple-mobile-web-app-title" content="CaféPlan Pro">
    <meta name="description" content="Sistema completo de gestão rural para produtores de café">
    
    <!-- PWA Icons -->
    <link rel="icon" type="image/png" sizes="192x192" href="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTkyIiBoZWlnaHQ9IjE5MiIgdmlld0JveD0iMCAwIDE5MiAxOTIiIGZpbGw9Im5vbmUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+CjxyZWN0IHdpZHRoPSIxOTIiIGhlaWdodD0iMTkyIiByeD0iMjQiIGZpbGw9IiMwNDc4NTciLz4KPHN2ZyB4PSI0OCIgeT0iNDgiIHdpZHRoPSI5NiIgaGVpZ2h0PSI5NiIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJ3aGl0ZSI+CjxwYXRoIGQ9Ik0xMiAyQzYuNDggMiAyIDYuNDggMiAxMnM0LjQ4IDEwIDEwIDEwIDEwLTQuNDggMTAtMTBTMTcuNTIgMiAxMiAyem0tMiAxNWwtNS01IDEuNDEtMS40MUwxMCAxNC4xN2w3LjU5LTcuNTlMMTkgOGwtOSA5eiIvPgo8L3N2Zz4KPC9zdmc+">
    <link rel="apple-touch-icon" href="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTkyIiBoZWlnaHQ9IjE5MiIgdmlld0JveD0iMCAwIDE5MiAxOTIiIGZpbGw9Im5vbmUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+CjxyZWN0IHdpZHRoPSIxOTIiIGhlaWdodD0iMTkyIiByeD0iMjQiIGZpbGw9IiMwNDc4NTciLz4KPHN2ZyB4PSI0OCIgeT0iNDgiIHdpZHRoPSI5NiIgaGVpZ2h0PSI5NiIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJ3aGl0ZSI+CjxwYXRoIGQ9Ik0xMiAyQzYuNDggMiAyIDYuNDggMiAxMnM0LjQ4IDEwIDEwIDEwIDEwLTQuNDggMTAtMTBTMTcuNTIgMiAxMiAyem0tMiAxNWwtNS01IDEuNDEtMS40MUwxMCAxNC4xN2w3LjU5LTcuNTlMMTkgOGwtOSA5eiIvPgo8L3N2Zz4KPC9zdmc+">
    
    <!-- PWA Manifest -->
    <link rel="manifest" href="data:application/json;base64,ewogICJuYW1lIjogIkNhZsOpUGxhbiBQcm8gLSBHZXN0w6NvIFJ1cmFsIENvbXBsZXRhIiwKICAic2hvcnRfbmFtZSI6ICJDYWbDqVBsYW4gUHJvIiwKICAiZGVzY3JpcHRpb24iOiAiU2lzdGVtYSBjb21wbGV0byBkZSBnZXN0w6NvIHJ1cmFsIHBhcmEgcHJvZHV0b3JlcyBkZSBjYWbDqSIsCiAgInN0YXJ0X3VybCI6ICIuLyIsCiAgImRpc3BsYXkiOiAic3RhbmRhbG9uZSIsCiAgInRoZW1lX2NvbG9yIjogIiMwNDc4NTciLAogICJiYWNrZ3JvdW5kX2NvbG9yIjogIiNmOWZhZmIiLAogICJvcmllbnRhdGlvbiI6ICJwb3J0cmFpdCIsCiAgImljb25zIjogWwogICAgewogICAgICAic3JjIjogImRhdGE6aW1hZ2Uvc3ZnK3htbDtiYXNlNjQsUEhOMlp5QjNhV1IwYUQwaU1Ua3lJaUJvWldsbmFIUTlJakU1TWlJZ2RtbGxkMEp2ZUQwaU1DQXdJREU1TWlBeE9USWlJR1pwYkd3OUltNXZibVVpSUhodGJHNXpQU0pvZEhSd09pOHZkM2QzTG5jekxtOXlaeTh5TURBd0wzTjJaeUkrQ2p4eVpXTjBJSGRwWkhSb1BTSXhPVElpSUdobGFXZG9kRDBpTVRreUlpQnllRDBpTWpRaUlHWnBiR3c5SWlNd05EYzROVGNpTHo0S1BITjJaeUI0UFNJME9DSWdlVDBpTkRnaUlIZHBaSFJvUFNJNU5pSWdhR1ZwWjJoMFBTSTVOaUlnZG1sbGQwSnZlRDBpTUNBd0lESTBJREkwSWlCbWFXeHNQU0ozYUdsMFpTSStDanh3WVhSb0lHUTlTVTB4TWlBeVF6WXVORGdnTWlBeUlEWXVORGdnTWlBeE1uTTBMalE0SURFd0lERXdJREV3SURFd0xUUXVORGdnTVRBdE1UQlRNVGN1TlRJZ01pQXhNaUF5ZW0wdE1pQXhOV3d0TlMwMUlERXVOREV0TVM0ME1VdzVNQ0F4TkM0eE4ydzNMalU1TFRjdU5UbE1NVGtnT0d3dE9TQTVlaUl2UGdvOEwzTjJaejRLUEM5emRtYysiLAogICAgICAic2l6ZXMiOiAiMTkyeDE5MiIsCiAgICAgICJ0eXBlIjogImltYWdlL3N2Zyt4bWwiCiAgICB9LAogICAgewogICAgICAic3JjIjogImRhdGE6aW1hZ2Uvc3ZnK3htbDtiYXNlNjQsUEhOMlp5QjNhV1IwYUQwaU5URXlJaUJvWldsbmFIUTlJalV4TWlJZ2RtbGxkMEp2ZUQwaU1DQXdJRFV4TWlBMU1USWlJR1pwYkd3OUltNXZibVVpSUhodGJHNXpQU0pvZEhSd09pOHZkM2QzTG5jekxtOXlaeTh5TURBd0wzTjJaeUkrQ2p4eVpXTjBJSGRwWkhSb1BTSTFNVElpSUdobGFXZG9kRDBpTlRFeUlpQnllRDBpTmpRaUlHWnBiR3c5SWlNd05EYzROVGNpTHo0S1BITjJaeUI0UFNJeE1qZ2lJSGs5SWpFeU9DSWdkMmxrZEdnOUlqSTFOaUlnYUdWcFoyaDBQU0l5TlRZaUlIWnBaWGRDYjNnOUlqQWdNQ0F5TkNBeU5DSWdabWxzYkQwaWQyaHBkR1VpUGdvOGNHRjBhQ0JrUFVsdE1USWdNa00yTGpRNElESWdNaUEyTGpRNElESWdNVEp6TkM0ME9DQXhNQ0F4TUNBeE1DQXhNQzAwTGpRNElERXdMVEV3VXpFM0xqVXlJRElnTVRJZ01tcHRMVElnTVRWc0xUVXROeUF4TGpReExURXVOREZNTVRBZ01UUXVNVGRzTnk0MU9TMDNMalU1VERFNUlEaHNMVGtnT1hvaUx6NEtQQzl6ZG1jK0Nqd3ZjM1puUGc9PSIsCiAgICAgICJzaXplcyI6ICI1MTJ4NTEyIiwKICAgICAgInR5cGUiOiAiaW1hZ2Uvc3ZnK3htbCIKICAgIH0KICBdCn0=">
    
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap');
        body { 
            font-family: 'Inter', sans-serif; 
            -webkit-font-smoothing: antialiased;
            -moz-osx-font-smoothing: grayscale;
            overscroll-behavior: none;
        }
        .tab-active { background: linear-gradient(135deg, #059669 0%, #047857 100%); color: white; }
        .card-hover:hover { transform: translateY(-2px); box-shadow: 0 10px 25px rgba(0,0,0,0.1); }
        .gradient-bg { background: linear-gradient(135deg, #065f46 0%, #047857 50%, #059669 100%); }
        .weather-card { background: linear-gradient(135deg, #3b82f6 0%, #1d4ed8 100%); }
        .task-priority-high { border-left: 4px solid #ef4444; }
        .task-priority-medium { border-left: 4px solid #f59e0b; }
        .task-priority-low { border-left: 4px solid #10b981; }
        
        /* PWA Styles */
        .pwa-install-banner {
            background: linear-gradient(135deg, #059669 0%, #047857 100%);
            color: white;
            padding: 12px 16px;
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            z-index: 1000;
            display: flex;
            align-items: center;
            justify-content: space-between;
            font-size: 14px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }
        
        /* Mobile optimizations */
        @media (max-width: 768px) {
            .container { padding-left: 12px; padding-right: 12px; }
            .tab-btn { font-size: 11px; padding: 8px 12px; }
            .grid { gap: 12px; }
        }
        
        /* Touch improvements */
        button, .tab-btn, input, select, textarea {
            touch-action: manipulation;
        }
        
        /* Prevent zoom on input focus */
        input, select, textarea {
            font-size: 16px;
        }
        
        @media (max-width: 768px) {
            input, select, textarea {
                font-size: 16px;
            }
        }
    </style>
</head>
<body class="bg-gray-50 min-h-screen">
    <!-- PWA Install Banner -->
    <div id="installBanner" class="hidden bg-gradient-to-r from-green-600 to-green-700 text-white px-4 py-3 shadow-lg">
        <div class="container mx-auto flex items-center justify-between">
            <div class="flex items-center space-x-3">
                <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24">
                    <path d="M19 9h-4V3H9v6H5l7 7 7-7zM5 18v2h14v-2H5z"/>
                </svg>
                <div>
                    <p class="font-medium">📱 Instalar CaféPlan Pro</p>
                    <p class="text-sm text-green-100">Instale o app no seu celular para acesso rápido e offline</p>
                </div>
            </div>
            <div class="flex items-center space-x-2">
                <button onclick="installPWA()" class="bg-white text-green-600 px-4 py-2 rounded-lg font-medium hover:bg-green-50 transition-colors">
                    Instalar
                </button>
                <button onclick="dismissInstallBanner()" class="text-green-100 hover:text-white p-2">
                    <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                        <path d="M19 6.41L17.59 5 12 10.59 6.41 5 5 6.41 10.59 12 5 17.59 6.41 19 12 13.41 17.59 19 19 17.59 13.41 12z"/>
                    </svg>
                </button>
            </div>
        </div>
    </div>

    <!-- Header -->
    <header class="gradient-bg text-white shadow-lg">
        <div class="container mx-auto px-4 py-6">
            <div class="flex items-center justify-between">
                <div class="flex items-center space-x-3">
                    <div class="bg-white/20 p-2 rounded-lg">
                        <svg class="w-8 h-8" fill="currentColor" viewBox="0 0 24 24">
                            <path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-2 15l-5-5 1.41-1.41L10 14.17l7.59-7.59L19 8l-9 9z"/>
                        </svg>
                    </div>
                    <div>
                        <h1 class="text-2xl font-bold">CaféPlan Pro</h1>
                        <p class="text-green-100 text-sm">Gestão Rural Inteligente</p>
                    </div>
                </div>
                <div class="flex items-center space-x-4">
                    <button id="installButtonHeader" onclick="installPWA()" class="hidden bg-white/20 hover:bg-white/30 px-3 py-2 rounded-lg text-sm font-medium transition-colors flex items-center space-x-2">
                        <svg class="w-4 h-4" fill="currentColor" viewBox="0 0 24 24">
                            <path d="M19 9h-4V3H9v6H5l7 7 7-7zM5 18v2h14v-2H5z"/>
                        </svg>
                        <span>Instalar App</span>
                    </button>
                    <div class="text-right">
                        <p class="text-sm text-green-100">Fazenda</p>
                        <p class="font-semibold" id="farmName">Minha Propriedade</p>
                        <p class="text-xs text-green-200" id="currentDateTime"></p>
                    </div>
                </div>
            </div>
        </div>
    </header>

    <!-- Navigation Tabs -->
    <nav class="bg-white shadow-sm border-b">
        <div class="container mx-auto px-4">
            <div class="flex space-x-1 overflow-x-auto">
                <button onclick="showTab('dashboard')" class="tab-btn tab-active px-4 py-3 text-xs font-medium rounded-t-lg whitespace-nowrap transition-all">
                    📊 Dashboard
                </button>
                <button onclick="showTab('area')" class="tab-btn px-4 py-3 text-xs font-medium rounded-t-lg whitespace-nowrap transition-all text-gray-600 hover:text-gray-800">
                    📏 Área & Plantio
                </button>
                <button onclick="showTab('irrigation')" class="tab-btn px-4 py-3 text-xs font-medium rounded-t-lg whitespace-nowrap transition-all text-gray-600 hover:text-gray-800">
                    💧 Irrigação
                </button>
                <button onclick="showTab('fertilizer')" class="tab-btn px-4 py-3 text-xs font-medium rounded-t-lg whitespace-nowrap transition-all text-gray-600 hover:text-gray-800">
                    🌱 Adubação
                </button>
                <button onclick="showTab('finance')" class="tab-btn px-4 py-3 text-xs font-medium rounded-t-lg whitespace-nowrap transition-all text-gray-600 hover:text-gray-800">
                    💰 Financeiro
                </button>
                <button onclick="showTab('tasks')" class="tab-btn px-4 py-3 text-xs font-medium rounded-t-lg whitespace-nowrap transition-all text-gray-600 hover:text-gray-800">
                    ✅ Tarefas
                </button>
                <button onclick="showTab('inventory')" class="tab-btn px-4 py-3 text-xs font-medium rounded-t-lg whitespace-nowrap transition-all text-gray-600 hover:text-gray-800">
                    📦 Estoque
                </button>
                <button onclick="showTab('equipment')" class="tab-btn px-4 py-3 text-xs font-medium rounded-t-lg whitespace-nowrap transition-all text-gray-600 hover:text-gray-800">
                    🚜 Equipamentos
                </button>
                <button onclick="showTab('weather')" class="tab-btn px-4 py-3 text-xs font-medium rounded-t-lg whitespace-nowrap transition-all text-gray-600 hover:text-gray-800">
                    🌤️ Clima
                </button>
                <button onclick="showTab('harvest')" class="tab-btn px-4 py-3 text-xs font-medium rounded-t-lg whitespace-nowrap transition-all text-gray-600 hover:text-gray-800">
                    ☕ Colheita
                </button>
                <button onclick="showTab('reports')" class="tab-btn px-4 py-3 text-xs font-medium rounded-t-lg whitespace-nowrap transition-all text-gray-600 hover:text-gray-800">
                    📈 Relatórios
                </button>
                <button onclick="showTab('calculator')" class="tab-btn px-4 py-3 text-xs font-medium rounded-t-lg whitespace-nowrap transition-all text-gray-600 hover:text-gray-800">
                    🧮 Calculadoras
                </button>
                <button onclick="showTab('employees')" class="tab-btn px-4 py-3 text-xs font-medium rounded-t-lg whitespace-nowrap transition-all text-gray-600 hover:text-gray-800">
                    👥 Funcionários
                </button>
                <button onclick="showTab('settings')" class="tab-btn px-4 py-3 text-xs font-medium rounded-t-lg whitespace-nowrap transition-all text-gray-600 hover:text-gray-800">
                    ⚙️ Configurações
                </button>
            </div>
        </div>
    </nav>

    <!-- Main Content -->
    <main class="container mx-auto px-4 py-6">
        <!-- Dashboard Tab -->
        <div id="dashboard" class="tab-content">
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6 mb-8">
                <div class="bg-white p-6 rounded-xl shadow-sm card-hover transition-all">
                    <div class="flex items-center justify-between">
                        <div>
                            <p class="text-gray-600 text-sm">Área Total</p>
                            <p class="text-2xl font-bold text-green-600" id="totalArea">0</p>
                            <p class="text-xs text-gray-500">Alqueires Paulistas</p>
                        </div>
                        <div class="bg-green-100 p-3 rounded-lg">
                            <svg class="w-6 h-6 text-green-600" fill="currentColor" viewBox="0 0 24 24">
                                <path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z"/>
                            </svg>
                        </div>
                    </div>
                </div>

                <div class="bg-white p-6 rounded-xl shadow-sm card-hover transition-all">
                    <div class="flex items-center justify-between">
                        <div>
                            <p class="text-gray-600 text-sm">Pés de Café</p>
                            <p class="text-2xl font-bold text-blue-600" id="totalPlants">0</p>
                            <p class="text-xs text-gray-500">Total plantado</p>
                        </div>
                        <div class="bg-blue-100 p-3 rounded-lg">
                            <svg class="w-6 h-6 text-blue-600" fill="currentColor" viewBox="0 0 24 24">
                                <path d="M17,8C8,10 5.9,16.17 3.82,21.34L5.71,22L6.66,19.7C7.14,19.87 7.64,20 8,20C19,20 22,3 22,3C21,5 14,5.25 9,6.25C4,7.25 2,11.5 2,13.5C2,15.5 3.75,17.25 3.75,17.25C7,8 17,8 17,8Z"/>
                            </svg>
                        </div>
                    </div>
                </div>

                <div class="bg-white p-6 rounded-xl shadow-sm card-hover transition-all">
                    <div class="flex items-center justify-between">
                        <div>
                            <p class="text-gray-600 text-sm">Receita Mensal</p>
                            <p class="text-2xl font-bold text-emerald-600" id="monthlyRevenue">R$ 0</p>
                            <p class="text-xs text-gray-500">Este mês</p>
                        </div>
                        <div class="bg-emerald-100 p-3 rounded-lg">
                            <svg class="w-6 h-6 text-emerald-600" fill="currentColor" viewBox="0 0 24 24">
                                <path d="M7,15H9C9,16.08 10.37,17 12,17C13.63,17 15,16.08 15,15C15,13.9 13.96,13.5 11.76,12.97C9.64,12.44 7,11.78 7,9C7,7.21 8.47,5.69 10.5,5.18V3H13.5V5.18C15.53,5.69 17,7.21 17,9H15C15,7.92 13.63,7 12,7C10.37,7 9,7.92 9,9C9,10.1 10.04,10.5 12.24,11.03C14.36,11.56 17,12.22 17,15C17,16.79 15.53,18.31 13.5,18.82V21H10.5V18.82C8.47,18.31 7,16.79 7,15Z"/>
                            </svg>
                        </div>
                    </div>
                </div>

                <div class="bg-white p-6 rounded-xl shadow-sm card-hover transition-all">
                    <div class="flex items-center justify-between">
                        <div>
                            <p class="text-gray-600 text-sm">Tarefas Pendentes</p>
                            <p class="text-2xl font-bold text-orange-600" id="pendingTasks">0</p>
                            <p class="text-xs text-gray-500">Para hoje</p>
                        </div>
                        <div class="bg-orange-100 p-3 rounded-lg">
                            <svg class="w-6 h-6 text-orange-600" fill="currentColor" viewBox="0 0 24 24">
                                <path d="M19,3H5C3.89,3 3,3.89 3,5V19A2,2 0 0,0 5,21H19A2,2 0 0,0 21,19V5C21,3.89 20.1,3 19,3M16.5,16L15.5,17L12,13.5L8.5,17L7.5,16L11,12.5L7.5,9L8.5,8L12,11.5L15.5,8L16.5,9L13,12.5L16.5,16Z"/>
                            </svg>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Weather Widget -->
            <div class="grid grid-cols-1 lg:grid-cols-3 gap-6 mb-8">
                <div class="weather-card text-white p-6 rounded-xl shadow-sm">
                    <h3 class="text-lg font-semibold mb-4">🌤️ Clima Hoje</h3>
                    <div class="flex items-center justify-between">
                        <div>
                            <p class="text-3xl font-bold" id="temperature">25°C</p>
                            <p class="text-blue-100">Parcialmente nublado</p>
                        </div>
                        <div class="text-right">
                            <p class="text-sm">Umidade: <span id="humidity">65%</span></p>
                            <p class="text-sm">Vento: <span id="windSpeed">12 km/h</span></p>
                            <p class="text-sm">Chuva: <span id="rainChance">30%</span></p>
                        </div>
                    </div>
                </div>

                <div class="bg-white p-6 rounded-xl shadow-sm col-span-2">
                    <h3 class="text-lg font-semibold mb-4">📋 Próximas Tarefas</h3>
                    <div id="upcomingTasks" class="space-y-2">
                        <p class="text-gray-500 text-sm">Nenhuma tarefa pendente</p>
                    </div>
                </div>
            </div>

            <!-- Reminders and Alerts -->
            <div class="bg-white rounded-xl shadow-sm p-6 mb-6">
                <div class="flex justify-between items-center mb-4">
                    <h3 class="text-lg font-semibold">🔔 Lembretes e Alertas</h3>
                    <button onclick="showReminderSettings()" class="text-blue-600 hover:text-blue-800 text-sm">
                        ⚙️ Configurar
                    </button>
                </div>
                <div id="remindersList" class="space-y-2">
                    <p class="text-gray-500 text-sm">Carregando lembretes...</p>
                </div>
            </div>

            <!-- Quick Actions -->
            <div class="bg-white rounded-xl shadow-sm p-6">
                <h3 class="text-lg font-semibold mb-4">Ações Rápidas</h3>
                <div class="grid grid-cols-2 md:grid-cols-6 gap-4">
                    <button onclick="showTab('area')" class="p-4 bg-green-50 rounded-lg hover:bg-green-100 transition-colors">
                        <div class="text-2xl mb-2">📏</div>
                        <p class="text-sm font-medium">Calcular Área</p>
                    </button>
                    <button onclick="showTab('tasks')" class="p-4 bg-blue-50 rounded-lg hover:bg-blue-100 transition-colors">
                        <div class="text-2xl mb-2">✅</div>
                        <p class="text-sm font-medium">Nova Tarefa</p>
                    </button>
                    <button onclick="showTab('inventory')" class="p-4 bg-yellow-50 rounded-lg hover:bg-yellow-100 transition-colors">
                        <div class="text-2xl mb-2">📦</div>
                        <p class="text-sm font-medium">Estoque</p>
                    </button>
                    <button onclick="showTab('harvest')" class="p-4 bg-red-50 rounded-lg hover:bg-red-100 transition-colors">
                        <div class="text-2xl mb-2">☕</div>
                        <p class="text-sm font-medium">Colheita</p>
                    </button>
                    <button onclick="showTab('finance')" class="p-4 bg-purple-50 rounded-lg hover:bg-purple-100 transition-colors">
                        <div class="text-2xl mb-2">💰</div>
                        <p class="text-sm font-medium">Financeiro</p>
                    </button>
                    <button onclick="showTab('reports')" class="p-4 bg-indigo-50 rounded-lg hover:bg-indigo-100 transition-colors">
                        <div class="text-2xl mb-2">📈</div>
                        <p class="text-sm font-medium">Relatórios</p>
                    </button>
                </div>
            </div>
        </div>

        <!-- Area & Planting Tab -->
        <div id="area" class="tab-content hidden">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-6">
                <!-- Area Calculator -->
                <div class="bg-white rounded-xl shadow-sm p-6">
                    <h3 class="text-lg font-semibold mb-4">📏 Calculadora de Área</h3>
                    <div class="space-y-4">
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Comprimento (metros)</label>
                            <input type="number" id="length" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent" placeholder="Ex: 1000">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Largura (metros)</label>
                            <input type="number" id="width" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent" placeholder="Ex: 500">
                        </div>
                        <button onclick="calculateArea()" class="w-full bg-green-600 text-white py-3 rounded-lg hover:bg-green-700 transition-colors font-medium">
                            Calcular Área
                        </button>
                        <div id="areaResult" class="hidden bg-green-50 p-4 rounded-lg">
                            <p class="text-sm text-gray-600">Área calculada:</p>
                            <p class="text-lg font-semibold text-green-600" id="areaValue"></p>
                            <p class="text-sm text-gray-500" id="areaHectares"></p>
                        </div>
                    </div>
                </div>

                <!-- Planting Calculator -->
                <div class="bg-white rounded-xl shadow-sm p-6">
                    <h3 class="text-lg font-semibold mb-4">🌱 Calculadora de Plantio</h3>
                    <div class="space-y-4">
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Área (Alqueires Paulistas)</label>
                            <input type="number" id="plantingArea" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent" placeholder="Ex: 5">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Variedade do café</label>
                            <select id="coffeeVariety" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent">
                                <option value="arabica">Arábica</option>
                                <option value="robusta">Robusta</option>
                                <option value="bourbon">Bourbon</option>
                                <option value="catuai">Catuaí</option>
                                <option value="mundo-novo">Mundo Novo</option>
                            </select>
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Espaçamento entre ruas (metros)</label>
                            <input type="number" id="rowSpacing" value="3.5" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Espaçamento entre plantas (metros)</label>
                            <input type="number" id="plantSpacing" value="0.7" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent">
                        </div>
                        <button onclick="calculatePlanting()" class="w-full bg-blue-600 text-white py-3 rounded-lg hover:bg-blue-700 transition-colors font-medium">
                            Calcular Mudas Necessárias
                        </button>
                        <div id="plantingResult" class="hidden bg-blue-50 p-4 rounded-lg">
                            <p class="text-sm text-gray-600">Mudas necessárias:</p>
                            <p class="text-lg font-semibold text-blue-600" id="seedlingsNeeded"></p>
                            <p class="text-sm text-gray-500" id="plantingDensity"></p>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Planting Records -->
            <div class="mt-6 bg-white rounded-xl shadow-sm p-6">
                <div class="flex justify-between items-center mb-4">
                    <h3 class="text-lg font-semibold">📋 Registro de Plantios</h3>
                    <button onclick="addPlantingRecord()" class="bg-green-600 text-white px-4 py-2 rounded-lg hover:bg-green-700 transition-colors">
                        + Novo Plantio
                    </button>
                </div>
                <div id="plantingRecords" class="space-y-3">
                    <p class="text-gray-500 text-sm">Nenhum plantio registrado ainda</p>
                </div>
            </div>
        </div>

        <!-- Irrigation Tab -->
        <div id="irrigation" class="tab-content hidden">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-6">
                <!-- Irrigation Calculator -->
                <div class="bg-white rounded-xl shadow-sm p-6">
                    <h3 class="text-lg font-semibold mb-4">💧 Calculadora de Irrigação</h3>
                    <div class="space-y-4">
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Área a irrigar (Alqueires)</label>
                            <input type="number" id="irrigationArea" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Ex: 3">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Lâmina d'água (mm/dia)</label>
                            <input type="number" id="waterDepth" value="5" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Eficiência do sistema (%)</label>
                            <input type="number" id="efficiency" value="85" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                        </div>
                        <button onclick="calculateIrrigation()" class="w-full bg-blue-600 text-white py-3 rounded-lg hover:bg-blue-700 transition-colors font-medium">
                            Calcular Necessidade Hídrica
                        </button>
                        <div id="irrigationResult" class="hidden bg-blue-50 p-4 rounded-lg">
                            <p class="text-sm text-gray-600">Volume necessário:</p>
                            <p class="text-lg font-semibold text-blue-600" id="waterVolume"></p>
                            <p class="text-sm text-gray-500" id="irrigationTime"></p>
                        </div>
                    </div>
                </div>

                <!-- Irrigation Schedule -->
                <div class="bg-white rounded-xl shadow-sm p-6">
                    <h3 class="text-lg font-semibold mb-4">📅 Cronograma de Irrigação</h3>
                    <div class="space-y-4">
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Setor</label>
                            <input type="text" id="irrigationSector" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Ex: Setor A">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Horário de início</label>
                            <input type="time" id="irrigationTimeSchedule" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Duração (horas)</label>
                            <input type="number" id="irrigationDuration" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Ex: 2">
                        </div>
                        <button onclick="addIrrigationSchedule()" class="w-full bg-blue-600 text-white py-3 rounded-lg hover:bg-blue-700 transition-colors font-medium">
                            Adicionar ao Cronograma
                        </button>
                    </div>
                    <div id="irrigationSchedule" class="mt-4 space-y-2">
                        <p class="text-gray-500 text-sm">Nenhuma irrigação agendada</p>
                    </div>
                </div>
            </div>
        </div>

        <!-- Fertilizer Tab -->
        <div id="fertilizer" class="tab-content hidden">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-6">
                <!-- Fertilizer Calculator -->
                <div class="bg-white rounded-xl shadow-sm p-6">
                    <h3 class="text-lg font-semibold mb-4">🌱 Calculadora de Adubação</h3>
                    <div class="space-y-4">
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Área (Alqueires)</label>
                            <input type="number" id="fertilizerArea" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent" placeholder="Ex: 5">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Tipo de adubo</label>
                            <select id="fertilizerType" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent">
                                <option value="npk">NPK 20-05-20</option>
                                <option value="organic">Orgânico</option>
                                <option value="urea">Ureia</option>
                                <option value="superfosfato">Superfosfato</option>
                            </select>
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Dosagem (kg/alqueire)</label>
                            <input type="number" id="fertilizerDose" value="300" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent">
                        </div>
                        <button onclick="calculateFertilizer()" class="w-full bg-green-600 text-white py-3 rounded-lg hover:bg-green-700 transition-colors font-medium">
                            Calcular Quantidade
                        </button>
                        <div id="fertilizerResult" class="hidden bg-green-50 p-4 rounded-lg">
                            <p class="text-sm text-gray-600">Quantidade total:</p>
                            <p class="text-lg font-semibold text-green-600" id="fertilizerAmount"></p>
                            <p class="text-sm text-gray-500" id="fertilizerCost"></p>
                        </div>
                    </div>
                </div>

                <!-- Fertilization Schedule -->
                <div class="bg-white rounded-xl shadow-sm p-6">
                    <h3 class="text-lg font-semibold mb-4">📋 Cronograma de Adubação</h3>
                    <div class="space-y-4">
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Data da aplicação</label>
                            <input type="date" id="fertilizerDate" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Setor</label>
                            <input type="text" id="fertilizerSector" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent" placeholder="Ex: Talhão 1">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Observações</label>
                            <textarea id="fertilizerNotes" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent" rows="3" placeholder="Ex: Aplicar após chuva"></textarea>
                        </div>
                        <button onclick="addFertilizerSchedule()" class="w-full bg-green-600 text-white py-3 rounded-lg hover:bg-green-700 transition-colors font-medium">
                            Adicionar ao Cronograma
                        </button>
                    </div>
                    <div id="fertilizerSchedule" class="mt-4 space-y-2">
                        <p class="text-gray-500 text-sm">Nenhuma adubação agendada</p>
                    </div>
                </div>
            </div>
        </div>

        <!-- Finance Tab -->
        <div id="finance" class="tab-content hidden">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-6">
                <!-- Add Revenue -->
                <div class="bg-white rounded-xl shadow-sm p-6">
                    <h3 class="text-lg font-semibold mb-4 text-green-600">💰 Adicionar Receita</h3>
                    <div class="space-y-4">
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Descrição</label>
                            <input type="text" id="revenueDescription" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent" placeholder="Ex: Venda de café">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Valor (R$)</label>
                            <input type="number" id="revenueAmount" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent" placeholder="Ex: 15000">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Data</label>
                            <input type="date" id="revenueDate" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent">
                        </div>
                        <button onclick="addRevenue()" class="w-full bg-green-600 text-white py-3 rounded-lg hover:bg-green-700 transition-colors font-medium">
                            Adicionar Receita
                        </button>
                    </div>
                </div>

                <!-- Add Expense -->
                <div class="bg-white rounded-xl shadow-sm p-6">
                    <h3 class="text-lg font-semibold mb-4 text-red-600">💸 Adicionar Despesa</h3>
                    <div class="space-y-4">
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Descrição</label>
                            <input type="text" id="expenseDescription" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-red-500 focus:border-transparent" placeholder="Ex: Compra de adubo">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Valor (R$)</label>
                            <input type="number" id="expenseAmount" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-red-500 focus:border-transparent" placeholder="Ex: 5000">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Categoria</label>
                            <select id="expenseCategory" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-red-500 focus:border-transparent">
                                <option value="insumos">Insumos</option>
                                <option value="mao-obra">Mão de obra</option>
                                <option value="combustivel">Combustível</option>
                                <option value="manutencao">Manutenção</option>
                                <option value="outros">Outros</option>
                            </select>
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Data</label>
                            <input type="date" id="expenseDate" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-red-500 focus:border-transparent">
                        </div>
                        <button onclick="addExpense()" class="w-full bg-red-600 text-white py-3 rounded-lg hover:bg-red-700 transition-colors font-medium">
                            Adicionar Despesa
                        </button>
                    </div>
                </div>
            </div>

            <!-- Financial Summary -->
            <div class="mt-6 bg-white rounded-xl shadow-sm p-6">
                <h3 class="text-lg font-semibold mb-4">📊 Resumo Financeiro</h3>
                <div class="grid grid-cols-1 md:grid-cols-3 gap-4 mb-6">
                    <div class="bg-green-50 p-4 rounded-lg">
                        <p class="text-sm text-gray-600">Total Receitas</p>
                        <p class="text-xl font-bold text-green-600" id="totalRevenue">R$ 0,00</p>
                    </div>
                    <div class="bg-red-50 p-4 rounded-lg">
                        <p class="text-sm text-gray-600">Total Despesas</p>
                        <p class="text-xl font-bold text-red-600" id="totalExpenses">R$ 0,00</p>
                    </div>
                    <div class="bg-blue-50 p-4 rounded-lg">
                        <p class="text-sm text-gray-600">Lucro Líquido</p>
                        <p class="text-xl font-bold text-blue-600" id="netProfit">R$ 0,00</p>
                    </div>
                </div>
                <div id="financialRecords" class="space-y-2">
                    <p class="text-gray-500 text-sm">Nenhuma movimentação financeira registrada</p>
                </div>
            </div>
        </div>

        <!-- Tasks Tab -->
        <div id="tasks" class="tab-content hidden">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-6">
                <!-- Add Task -->
                <div class="bg-white rounded-xl shadow-sm p-6">
                    <h3 class="text-lg font-semibold mb-4">✅ Nova Tarefa</h3>
                    <div class="space-y-4">
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Título da tarefa</label>
                            <input type="text" id="taskTitle" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Ex: Aplicar herbicida no talhão 3">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Categoria</label>
                            <select id="taskCategory" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                                <option value="plantio">Plantio</option>
                                <option value="irrigacao">Irrigação</option>
                                <option value="adubacao">Adubação</option>
                                <option value="pulverizacao">Pulverização</option>
                                <option value="colheita">Colheita</option>
                                <option value="manutencao">Manutenção</option>
                                <option value="administrativo">Administrativo</option>
                            </select>
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Prioridade</label>
                            <select id="taskPriority" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                                <option value="low">Baixa</option>
                                <option value="medium">Média</option>
                                <option value="high">Alta</option>
                            </select>
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Data prevista</label>
                            <input type="date" id="taskDate" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Responsável</label>
                            <input type="text" id="taskResponsible" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Ex: João Silva">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Observações</label>
                            <textarea id="taskNotes" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" rows="3" placeholder="Detalhes adicionais..."></textarea>
                        </div>
                        <button onclick="addTask()" class="w-full bg-blue-600 text-white py-3 rounded-lg hover:bg-blue-700 transition-colors font-medium">
                            Adicionar Tarefa
                        </button>
                    </div>
                </div>

                <!-- Task Filters -->
                <div class="bg-white rounded-xl shadow-sm p-6">
                    <h3 class="text-lg font-semibold mb-4">🔍 Filtros</h3>
                    <div class="space-y-4">
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Status</label>
                            <select id="taskFilter" onchange="filterTasks()" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                                <option value="all">Todas</option>
                                <option value="pending">Pendentes</option>
                                <option value="completed">Concluídas</option>
                                <option value="overdue">Atrasadas</option>
                            </select>
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Categoria</label>
                            <select id="categoryFilter" onchange="filterTasks()" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                                <option value="all">Todas</option>
                                <option value="plantio">Plantio</option>
                                <option value="irrigacao">Irrigação</option>
                                <option value="adubacao">Adubação</option>
                                <option value="pulverizacao">Pulverização</option>
                                <option value="colheita">Colheita</option>
                                <option value="manutencao">Manutenção</option>
                                <option value="administrativo">Administrativo</option>
                            </select>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Task List -->
            <div class="mt-6 bg-white rounded-xl shadow-sm p-6">
                <h3 class="text-lg font-semibold mb-4">📋 Lista de Tarefas</h3>
                <div id="taskList" class="space-y-3">
                    <p class="text-gray-500 text-sm">Nenhuma tarefa cadastrada ainda</p>
                </div>
            </div>
        </div>

        <!-- Inventory Tab -->
        <div id="inventory" class="tab-content hidden">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-6">
                <!-- Add Inventory Item -->
                <div class="bg-white rounded-xl shadow-sm p-6">
                    <h3 class="text-lg font-semibold mb-4">📦 Adicionar Item ao Estoque</h3>
                    <div class="space-y-4">
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Nome do produto</label>
                            <input type="text" id="inventoryName" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent" placeholder="Ex: Adubo NPK 20-05-20">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Categoria</label>
                            <select id="inventoryCategory" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent">
                                <option value="fertilizantes">Fertilizantes</option>
                                <option value="defensivos">Defensivos</option>
                                <option value="sementes">Sementes/Mudas</option>
                                <option value="combustivel">Combustível</option>
                                <option value="ferramentas">Ferramentas</option>
                                <option value="equipamentos">Equipamentos</option>
                                <option value="outros">Outros</option>
                            </select>
                        </div>
                        <div class="grid grid-cols-2 gap-4">
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Quantidade</label>
                                <input type="number" id="inventoryQuantity" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent" placeholder="Ex: 50">
                            </div>
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Unidade</label>
                                <select id="inventoryUnit" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent">
                                    <option value="kg">Kg</option>
                                    <option value="litros">Litros</option>
                                    <option value="sacas">Sacas</option>
                                    <option value="unidades">Unidades</option>
                                    <option value="metros">Metros</option>
                                </select>
                            </div>
                        </div>
                        <div class="grid grid-cols-2 gap-4">
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Preço unitário (R$)</label>
                                <input type="number" id="inventoryPrice" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent" placeholder="Ex: 3.50">
                            </div>
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Estoque mínimo</label>
                                <input type="number" id="inventoryMinStock" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent" placeholder="Ex: 10">
                            </div>
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Fornecedor</label>
                            <input type="text" id="inventorySupplier" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent" placeholder="Ex: Agropecuária Silva">
                        </div>
                        <button onclick="addInventoryItem()" class="w-full bg-green-600 text-white py-3 rounded-lg hover:bg-green-700 transition-colors font-medium">
                            Adicionar ao Estoque
                        </button>
                    </div>
                </div>

                <!-- Inventory Summary -->
                <div class="bg-white rounded-xl shadow-sm p-6">
                    <h3 class="text-lg font-semibold mb-4">📊 Resumo do Estoque</h3>
                    <div class="grid grid-cols-2 gap-4 mb-6">
                        <div class="bg-blue-50 p-4 rounded-lg">
                            <p class="text-sm text-gray-600">Total de Itens</p>
                            <p class="text-xl font-bold text-blue-600" id="totalInventoryItems">0</p>
                        </div>
                        <div class="bg-red-50 p-4 rounded-lg">
                            <p class="text-sm text-gray-600">Estoque Baixo</p>
                            <p class="text-xl font-bold text-red-600" id="lowStockItems">0</p>
                        </div>
                    </div>
                    <div>
                        <h4 class="font-medium mb-2">🚨 Alertas de Estoque</h4>
                        <div id="stockAlerts" class="space-y-2">
                            <p class="text-sm text-gray-500">Nenhum alerta de estoque</p>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Inventory List -->
            <div class="mt-6 bg-white rounded-xl shadow-sm p-6">
                <div class="flex justify-between items-center mb-4">
                    <h3 class="text-lg font-semibold">📋 Lista de Estoque</h3>
                    <div class="flex space-x-2">
                        <select id="inventoryFilterCategory" onchange="filterInventory()" class="px-3 py-2 border border-gray-300 rounded-lg text-sm">
                            <option value="all">Todas as categorias</option>
                            <option value="fertilizantes">Fertilizantes</option>
                            <option value="defensivos">Defensivos</option>
                            <option value="sementes">Sementes/Mudas</option>
                            <option value="combustivel">Combustível</option>
                            <option value="ferramentas">Ferramentas</option>
                            <option value="equipamentos">Equipamentos</option>
                            <option value="outros">Outros</option>
                        </select>
                    </div>
                </div>
                <div id="inventoryList" class="space-y-3">
                    <p class="text-gray-500 text-sm">Nenhum item no estoque ainda</p>
                </div>
            </div>
        </div>

        <!-- Equipment Tab -->
        <div id="equipment" class="tab-content hidden">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-6">
                <!-- Add Equipment -->
                <div class="bg-white rounded-xl shadow-sm p-6">
                    <h3 class="text-lg font-semibold mb-4">🚜 Cadastrar Equipamento</h3>
                    <div class="space-y-4">
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Nome/Modelo</label>
                            <input type="text" id="equipmentName" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Ex: Trator Massey Ferguson 4275">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Tipo</label>
                            <select id="equipmentType" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                                <option value="trator">Trator</option>
                                <option value="pulverizador">Pulverizador</option>
                                <option value="colheitadeira">Colheitadeira</option>
                                <option value="implemento">Implemento</option>
                                <option value="bomba">Bomba d'água</option>
                                <option value="gerador">Gerador</option>
                                <option value="veiculo">Veículo</option>
                                <option value="outros">Outros</option>
                            </select>
                        </div>
                        <div class="grid grid-cols-2 gap-4">
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Ano</label>
                                <input type="number" id="equipmentYear" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Ex: 2020">
                            </div>
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Horas trabalhadas</label>
                                <input type="number" id="equipmentHours" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Ex: 1500">
                            </div>
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Próxima manutenção (horas)</label>
                            <input type="number" id="equipmentNextMaintenance" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Ex: 1600">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Status</label>
                            <select id="equipmentStatus" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                                <option value="operacional">Operacional</option>
                                <option value="manutencao">Em manutenção</option>
                                <option value="quebrado">Quebrado</option>
                                <option value="inativo">Inativo</option>
                            </select>
                        </div>
                        <button onclick="addEquipment()" class="w-full bg-blue-600 text-white py-3 rounded-lg hover:bg-blue-700 transition-colors font-medium">
                            Cadastrar Equipamento
                        </button>
                    </div>
                </div>

                <!-- Equipment Summary -->
                <div class="bg-white rounded-xl shadow-sm p-6">
                    <h3 class="text-lg font-semibold mb-4">📊 Status dos Equipamentos</h3>
                    <div class="grid grid-cols-2 gap-4 mb-6">
                        <div class="bg-green-50 p-4 rounded-lg">
                            <p class="text-sm text-gray-600">Operacionais</p>
                            <p class="text-xl font-bold text-green-600" id="operationalEquipment">0</p>
                        </div>
                        <div class="bg-red-50 p-4 rounded-lg">
                            <p class="text-sm text-gray-600">Precisam Manutenção</p>
                            <p class="text-xl font-bold text-red-600" id="maintenanceNeeded">0</p>
                        </div>
                    </div>
                    <div>
                        <h4 class="font-medium mb-2">🔧 Alertas de Manutenção</h4>
                        <div id="maintenanceAlerts" class="space-y-2">
                            <p class="text-sm text-gray-500">Nenhum alerta de manutenção</p>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Equipment List -->
            <div class="mt-6 bg-white rounded-xl shadow-sm p-6">
                <h3 class="text-lg font-semibold mb-4">🚜 Lista de Equipamentos</h3>
                <div id="equipmentList" class="space-y-3">
                    <p class="text-gray-500 text-sm">Nenhum equipamento cadastrado ainda</p>
                </div>
            </div>
        </div>

        <!-- Weather Tab -->
        <div id="weather" class="tab-content hidden">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-6">
                <!-- Current Weather -->
                <div class="weather-card text-white p-6 rounded-xl shadow-sm">
                    <h3 class="text-xl font-semibold mb-4">🌤️ Clima Atual</h3>
                    <div class="flex items-center justify-between mb-6">
                        <div>
                            <p class="text-4xl font-bold mb-2" id="currentTemp">25°C</p>
                            <p class="text-blue-100" id="weatherDescription">Parcialmente nublado</p>
                        </div>
                        <div class="text-6xl">☁️</div>
                    </div>
                    <div class="grid grid-cols-2 gap-4">
                        <div>
                            <p class="text-sm text-blue-100">Umidade</p>
                            <p class="text-lg font-semibold" id="currentHumidity">65%</p>
                        </div>
                        <div>
                            <p class="text-sm text-blue-100">Vento</p>
                            <p class="text-lg font-semibold" id="currentWind">12 km/h</p>
                        </div>
                        <div>
                            <p class="text-sm text-blue-100">Pressão</p>
                            <p class="text-lg font-semibold" id="currentPressure">1013 hPa</p>
                        </div>
                        <div>
                            <p class="text-sm text-blue-100">Chuva</p>
                            <p class="text-lg font-semibold" id="currentRain">30%</p>
                        </div>
                    </div>
                </div>

                <!-- Weather Recommendations -->
                <div class="bg-white rounded-xl shadow-sm p-6">
                    <h3 class="text-lg font-semibold mb-4">💡 Recomendações Agrícolas</h3>
                    <div id="weatherRecommendations" class="space-y-3">
                        <div class="bg-green-50 p-3 rounded-lg">
                            <p class="font-medium text-green-800">✅ Bom para irrigação</p>
                            <p class="text-sm text-green-600">Umidade adequada e sem previsão de chuva</p>
                        </div>
                        <div class="bg-yellow-50 p-3 rounded-lg">
                            <p class="font-medium text-yellow-800">⚠️ Atenção para pulverização</p>
                            <p class="text-sm text-yellow-600">Vento moderado, aguardar condições mais calmas</p>
                        </div>
                        <div class="bg-blue-50 p-3 rounded-lg">
                            <p class="font-medium text-blue-800">🌧️ Possível chuva</p>
                            <p class="text-sm text-blue-600">Adiar aplicações de defensivos</p>
                        </div>
                    </div>
                </div>
            </div>

            <!-- 7-Day Forecast -->
            <div class="mt-6 bg-white rounded-xl shadow-sm p-6">
                <h3 class="text-lg font-semibold mb-4">📅 Previsão para 7 dias</h3>
                <div class="grid grid-cols-1 md:grid-cols-7 gap-4" id="weeklyForecast">
                    <!-- Weekly forecast will be populated here -->
                </div>
            </div>
        </div>

        <!-- Harvest Tab -->
        <div id="harvest" class="tab-content hidden">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-6">
                <!-- Record Harvest -->
                <div class="bg-white rounded-xl shadow-sm p-6">
                    <h3 class="text-lg font-semibold mb-4">☕ Registrar Colheita</h3>
                    <div class="space-y-4">
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Data da colheita</label>
                            <input type="date" id="harvestDate" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Talhão/Setor</label>
                            <input type="text" id="harvestSector" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent" placeholder="Ex: Talhão 1">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Área colhida (Alqueires)</label>
                            <input type="number" id="harvestArea" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent" placeholder="Ex: 2.5">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Quantidade colhida (sacas)</label>
                            <input type="number" id="harvestQuantity" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent" placeholder="Ex: 150">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Qualidade do café</label>
                            <select id="harvestQuality" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent">
                                <option value="superior">Superior</option>
                                <option value="boa">Boa</option>
                                <option value="regular">Regular</option>
                                <option value="inferior">Inferior</option>
                            </select>
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Preço por saca (R$)</label>
                            <input type="number" id="harvestPrice" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent" placeholder="Ex: 450.00">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Observações</label>
                            <textarea id="harvestNotes" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent" rows="3" placeholder="Condições da colheita, umidade, etc."></textarea>
                        </div>
                        <button onclick="addHarvestRecord()" class="w-full bg-green-600 text-white py-3 rounded-lg hover:bg-green-700 transition-colors font-medium">
                            Registrar Colheita
                        </button>
                    </div>
                </div>

                <!-- Harvest Summary -->
                <div class="bg-white rounded-xl shadow-sm p-6">
                    <h3 class="text-lg font-semibold mb-4">📊 Resumo da Safra</h3>
                    <div class="grid grid-cols-2 gap-4 mb-6">
                        <div class="bg-green-50 p-4 rounded-lg">
                            <p class="text-sm text-gray-600">Total Colhido</p>
                            <p class="text-xl font-bold text-green-600" id="totalHarvested">0 sacas</p>
                        </div>
                        <div class="bg-blue-50 p-4 rounded-lg">
                            <p class="text-sm text-gray-600">Produtividade Média</p>
                            <p class="text-xl font-bold text-blue-600" id="averageProductivity">0 sc/alq</p>
                        </div>
                        <div class="bg-yellow-50 p-4 rounded-lg">
                            <p class="text-sm text-gray-600">Receita Total</p>
                            <p class="text-xl font-bold text-yellow-600" id="totalHarvestRevenue">R$ 0</p>
                        </div>
                        <div class="bg-purple-50 p-4 rounded-lg">
                            <p class="text-sm text-gray-600">Preço Médio</p>
                            <p class="text-xl font-bold text-purple-600" id="averagePrice">R$ 0/sc</p>
                        </div>
                    </div>
                    <button onclick="calculateHarvestProjection()" class="w-full bg-blue-600 text-white py-3 rounded-lg hover:bg-blue-700 transition-colors font-medium">
                        Calcular Projeção da Safra
                    </button>
                </div>
            </div>

            <!-- Harvest Records -->
            <div class="mt-6 bg-white rounded-xl shadow-sm p-6">
                <h3 class="text-lg font-semibold mb-4">📋 Histórico de Colheitas</h3>
                <div id="harvestRecords" class="space-y-3">
                    <p class="text-gray-500 text-sm">Nenhuma colheita registrada ainda</p>
                </div>
            </div>
        </div>

        <!-- Reports Tab -->
        <div id="reports" class="tab-content hidden">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-6">
                <!-- Report Generator -->
                <div class="bg-white rounded-xl shadow-sm p-6">
                    <h3 class="text-lg font-semibold mb-4">📈 Gerar Relatório</h3>
                    <div class="space-y-4">
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Tipo de relatório</label>
                            <select id="reportType" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                                <option value="financial">Financeiro</option>
                                <option value="production">Produção</option>
                                <option value="inventory">Estoque</option>
                                <option value="tasks">Tarefas</option>
                                <option value="equipment">Equipamentos</option>
                            </select>
                        </div>
                        <div class="grid grid-cols-2 gap-4">
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Data inicial</label>
                                <input type="date" id="reportStartDate" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                            </div>
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Data final</label>
                                <input type="date" id="reportEndDate" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                            </div>
                        </div>
                        <button onclick="generateReport()" class="w-full bg-blue-600 text-white py-3 rounded-lg hover:bg-blue-700 transition-colors font-medium">
                            Gerar Relatório
                        </button>
                    </div>
                </div>

                <!-- Quick Stats -->
                <div class="bg-white rounded-xl shadow-sm p-6">
                    <h3 class="text-lg font-semibold mb-4">📊 Estatísticas Rápidas</h3>
                    <div class="space-y-4">
                        <div class="flex justify-between items-center p-3 bg-gray-50 rounded-lg">
                            <span class="text-sm font-medium">Lucro este mês</span>
                            <span class="font-bold text-green-600" id="monthlyProfit">R$ 0</span>
                        </div>
                        <div class="flex justify-between items-center p-3 bg-gray-50 rounded-lg">
                            <span class="text-sm font-medium">Tarefas concluídas</span>
                            <span class="font-bold text-blue-600" id="completedTasksCount">0</span>
                        </div>
                        <div class="flex justify-between items-center p-3 bg-gray-50 rounded-lg">
                            <span class="text-sm font-medium">Equipamentos ativos</span>
                            <span class="font-bold text-purple-600" id="activeEquipmentCount">0</span>
                        </div>
                        <div class="flex justify-between items-center p-3 bg-gray-50 rounded-lg">
                            <span class="text-sm font-medium">Itens em estoque baixo</span>
                            <span class="font-bold text-red-600" id="lowStockCount">0</span>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Report Display -->
            <div class="mt-6 bg-white rounded-xl shadow-sm p-6">
                <h3 class="text-lg font-semibold mb-4">📋 Relatório Gerado</h3>
                <div id="reportDisplay" class="text-center text-gray-500 py-8">
                    Selecione um tipo de relatório e clique em "Gerar Relatório" para visualizar os dados.
                </div>
            </div>
        </div>

        <!-- Employees Tab -->
        <div id="employees" class="tab-content hidden">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-6">
                <!-- Add Employee -->
                <div class="bg-white rounded-xl shadow-sm p-6">
                    <h3 class="text-lg font-semibold mb-4">👥 Cadastrar Funcionário</h3>
                    <div class="space-y-4">
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Nome completo</label>
                            <input type="text" id="employeeName" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Ex: João Silva Santos">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Função</label>
                            <select id="employeeRole" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                                <option value="operador-campo">Operador de Campo</option>
                                <option value="tratorista">Tratorista</option>
                                <option value="aplicador">Aplicador de Defensivos</option>
                                <option value="colhedor">Colhedor</option>
                                <option value="colhedor-selecionador">Colhedor Selecionador</option>
                                <option value="irrigador">Irrigador</option>
                                <option value="podador">Podador</option>
                                <option value="mecanico">Mecânico</option>
                                <option value="eletricista">Eletricista</option>
                                <option value="soldador">Soldador</option>
                                <option value="motorista">Motorista</option>
                                <option value="operador-maquinas">Operador de Máquinas</option>
                                <option value="supervisor">Supervisor de Campo</option>
                                <option value="encarregado">Encarregado</option>
                                <option value="tecnico-agricola">Técnico Agrícola</option>
                                <option value="engenheiro">Engenheiro Agrônomo</option>
                                <option value="veterinario">Veterinário</option>
                                <option value="administrativo">Administrativo</option>
                                <option value="contador">Contador</option>
                                <option value="recursos-humanos">Recursos Humanos</option>
                                <option value="gerente">Gerente</option>
                                <option value="coordenador">Coordenador</option>
                                <option value="diretor">Diretor</option>
                                <option value="vigilante">Vigilante</option>
                                <option value="porteiro">Porteiro</option>
                                <option value="cozinheiro">Cozinheiro</option>
                                <option value="auxiliar-limpeza">Auxiliar de Limpeza</option>
                                <option value="jardineiro">Jardineiro</option>
                                <option value="caseiro">Caseiro</option>
                                <option value="outros">Outros</option>
                            </select>
                        </div>
                        <div class="grid grid-cols-2 gap-4">
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Salário (R$)</label>
                                <input type="number" id="employeeSalary" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Ex: 1500 (ou 0 para pagamento por produção)" min="0">
                            </div>
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Data de admissão</label>
                                <input type="date" id="employeeHireDate" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                            </div>
                        </div>
                        <div class="grid grid-cols-2 gap-4">
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">CPF</label>
                                <input type="text" id="employeeCPF" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Ex: 000.000.000-00">
                            </div>
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">RG</label>
                                <input type="text" id="employeeRG" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Ex: 00.000.000-0">
                            </div>
                        </div>
                        <div class="grid grid-cols-2 gap-4">
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Telefone</label>
                                <input type="tel" id="employeePhone" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Ex: (11) 99999-9999">
                            </div>
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Email</label>
                                <input type="email" id="employeeEmail" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Ex: joao@email.com">
                            </div>
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Endereço</label>
                            <input type="text" id="employeeAddress" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Ex: Rua das Flores, 123 - Centro">
                        </div>
                        <div class="grid grid-cols-3 gap-4">
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Data de Nascimento</label>
                                <input type="date" id="employeeBirthDate" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                            </div>
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Estado Civil</label>
                                <select id="employeeMaritalStatus" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                                    <option value="">Selecione</option>
                                    <option value="solteiro">Solteiro(a)</option>
                                    <option value="casado">Casado(a)</option>
                                    <option value="divorciado">Divorciado(a)</option>
                                    <option value="viuvo">Viúvo(a)</option>
                                    <option value="uniao-estavel">União Estável</option>
                                </select>
                            </div>
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Escolaridade</label>
                                <select id="employeeEducation" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                                    <option value="">Selecione</option>
                                    <option value="fundamental-incompleto">Fundamental Incompleto</option>
                                    <option value="fundamental-completo">Fundamental Completo</option>
                                    <option value="medio-incompleto">Médio Incompleto</option>
                                    <option value="medio-completo">Médio Completo</option>
                                    <option value="tecnico">Técnico</option>
                                    <option value="superior-incompleto">Superior Incompleto</option>
                                    <option value="superior-completo">Superior Completo</option>
                                    <option value="pos-graduacao">Pós-graduação</option>
                                </select>
                            </div>
                        </div>
                        <div class="grid grid-cols-2 gap-4">
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Banco</label>
                                <input type="text" id="employeeBank" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Ex: Banco do Brasil">
                            </div>
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Agência e Conta</label>
                                <input type="text" id="employeeBankAccount" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Ex: 1234-5 / 67890-1">
                            </div>
                        </div>
                        <div class="grid grid-cols-2 gap-4">
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Contato de Emergência</label>
                                <input type="text" id="employeeEmergencyContact" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Ex: Maria Silva">
                            </div>
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Telefone de Emergência</label>
                                <input type="tel" id="employeeEmergencyPhone" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Ex: (11) 88888-8888">
                            </div>
                        </div>
                        <div class="grid grid-cols-2 gap-4">
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Status</label>
                                <select id="employeeStatus" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                                    <option value="ativo">Ativo</option>
                                    <option value="ferias">Férias</option>
                                    <option value="afastado">Afastado</option>
                                    <option value="licenca">Licença</option>
                                    <option value="demitido">Demitido</option>
                                </select>
                            </div>
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Tipo de Contrato</label>
                                <select id="employeeContractType" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                                    <option value="clt">CLT</option>
                                    <option value="temporario">Temporário</option>
                                    <option value="terceirizado">Terceirizado</option>
                                    <option value="cooperado">Cooperado</option>
                                    <option value="autonomo">Autônomo</option>
                                    <option value="estagiario">Estagiário</option>
                                </select>
                            </div>
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Observações</label>
                            <textarea id="employeeNotes" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" rows="3" placeholder="Informações adicionais..."></textarea>
                        </div>
                        <button onclick="addEmployee()" class="w-full bg-blue-600 text-white py-3 rounded-lg hover:bg-blue-700 transition-colors font-medium">
                            Cadastrar Funcionário
                        </button>
                    </div>
                </div>

                <!-- Production Tracking -->
                <div class="bg-white rounded-xl shadow-sm p-6">
                    <h3 class="text-lg font-semibold mb-4">📊 Registrar Produção Diária</h3>
                    <div class="space-y-4">
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Funcionário</label>
                            <select id="productionEmployee" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                                <option value="">Selecione um funcionário</option>
                            </select>
                        </div>
                        <div class="grid grid-cols-2 gap-4">
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Data</label>
                                <input type="date" id="productionDate" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                            </div>
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Quantidade (sacas)</label>
                                <input type="number" id="productionQuantity" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Ex: 12" step="0.1">
                            </div>
                        </div>
                        <div class="grid grid-cols-2 gap-4">
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Setor/Talhão</label>
                                <input type="text" id="productionSector" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Ex: Talhão 1">
                            </div>
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Horas trabalhadas</label>
                                <input type="number" id="productionHours" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Ex: 8" step="0.5">
                            </div>
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Observações</label>
                            <input type="text" id="productionNotes" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Ex: Café cereja, qualidade boa">
                        </div>
                        <button onclick="addProductionRecord()" class="w-full bg-blue-600 text-white py-3 rounded-lg hover:bg-blue-700 transition-colors font-medium">
                            Registrar Produção
                        </button>
                    </div>
                    
                    <!-- Production Summary -->
                    <div class="mt-6 pt-6 border-t">
                        <h4 class="font-medium mb-3">📈 Resumo de Produção</h4>
                        <div class="grid grid-cols-2 gap-4">
                            <div class="bg-green-50 p-3 rounded-lg">
                                <p class="text-sm text-gray-600">Hoje</p>
                                <p class="text-lg font-bold text-green-600" id="todayProduction">0 sacas</p>
                            </div>
                            <div class="bg-blue-50 p-3 rounded-lg">
                                <p class="text-sm text-gray-600">Esta Semana</p>
                                <p class="text-lg font-bold text-blue-600" id="weekProduction">0 sacas</p>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Payroll Management -->
                <div class="bg-white rounded-xl shadow-sm p-6">
                    <h3 class="text-lg font-semibold mb-4">💰 Gerar Pagamento por Produção</h3>
                    <div class="space-y-4">
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Funcionário</label>
                            <select id="payrollEmployee" onchange="loadEmployeeProduction()" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent">
                                <option value="">Selecione um funcionário</option>
                            </select>
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Tipo de pagamento</label>
                            <select id="payrollType" onchange="togglePaymentFields()" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent">
                                <option value="salario">Salário</option>
                                <option value="hora-extra">Hora Extra</option>
                                <option value="bonus">Bônus</option>
                                <option value="adicional">Adicional</option>
                                <option value="decimo">13º Salário</option>
                                <option value="ferias">Férias</option>
                                <option value="producao-acumulada">Pagamento por Produção Acumulada</option>
                            </select>
                        </div>
                        
                        <!-- Campos para pagamento fixo -->
                        <div id="fixedPaymentFields" class="grid grid-cols-2 gap-4">
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Valor (R$)</label>
                                <input type="number" id="payrollAmount" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent" placeholder="Ex: 1500">
                            </div>
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Data do pagamento</label>
                                <input type="date" id="payrollDate" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent">
                            </div>
                        </div>
                        
                        <!-- Campos para pagamento por produção acumulada -->
                        <div id="accumulatedProductionFields" class="hidden space-y-4">
                            <div class="grid grid-cols-2 gap-4">
                                <div>
                                    <label class="block text-sm font-medium text-gray-700 mb-2">Período</label>
                                    <select id="productionPeriod" onchange="calculateAccumulatedProduction()" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent">
                                        <option value="week">Última Semana</option>
                                        <option value="biweekly">Últimas 2 Semanas</option>
                                        <option value="month">Último Mês</option>
                                        <option value="custom">Período Personalizado</option>
                                    </select>
                                </div>
                                <div>
                                    <label class="block text-sm font-medium text-gray-700 mb-2">Valor por saca (R$)</label>
                                    <input type="number" id="accumulatedPricePerBag" onchange="calculateAccumulatedProduction()" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent" placeholder="Ex: 8.50" step="0.01">
                                </div>
                            </div>
                            
                            <!-- Campos para período personalizado -->
                            <div id="customPeriodFields" class="hidden grid grid-cols-2 gap-4">
                                <div>
                                    <label class="block text-sm font-medium text-gray-700 mb-2">Data inicial</label>
                                    <input type="date" id="customStartDate" onchange="calculateAccumulatedProduction()" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent">
                                </div>
                                <div>
                                    <label class="block text-sm font-medium text-gray-700 mb-2">Data final</label>
                                    <input type="date" id="customEndDate" onchange="calculateAccumulatedProduction()" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent">
                                </div>
                            </div>
                            
                            <div class="bg-blue-50 p-4 rounded-lg">
                                <div class="grid grid-cols-3 gap-4 text-center">
                                    <div>
                                        <p class="text-sm text-gray-600">Sacas Acumuladas</p>
                                        <p class="text-lg font-bold text-blue-600" id="accumulatedBags">0</p>
                                    </div>
                                    <div>
                                        <p class="text-sm text-gray-600">Dias Trabalhados</p>
                                        <p class="text-lg font-bold text-blue-600" id="workingDays">0</p>
                                    </div>
                                    <div>
                                        <p class="text-sm text-gray-600">Total a Pagar</p>
                                        <p class="text-lg font-bold text-green-600" id="accumulatedTotal">R$ 0,00</p>
                                    </div>
                                </div>
                            </div>
                            
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Data do pagamento</label>
                                <input type="date" id="accumulatedPaymentDate" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent">
                            </div>
                        </div>
                        
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Referência</label>
                            <input type="text" id="payrollReference" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent" placeholder="Ex: Janeiro 2024">
                        </div>
                        <button onclick="addPayroll()" class="w-full bg-green-600 text-white py-3 rounded-lg hover:bg-green-700 transition-colors font-medium">
                            Registrar Pagamento
                        </button>
                    </div>
                    
                    <!-- Payroll Summary -->
                    <div class="mt-6 pt-6 border-t">
                        <h4 class="font-medium mb-3">📊 Resumo da Folha</h4>
                        <div class="grid grid-cols-2 gap-4">
                            <div class="bg-blue-50 p-3 rounded-lg">
                                <p class="text-sm text-gray-600">Total Funcionários</p>
                                <p class="text-lg font-bold text-blue-600" id="totalEmployees">0</p>
                            </div>
                            <div class="bg-green-50 p-3 rounded-lg">
                                <p class="text-sm text-gray-600">Folha Mensal</p>
                                <p class="text-lg font-bold text-green-600" id="monthlyPayroll">R$ 0</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Employee List -->
            <div class="mt-6 bg-white rounded-xl shadow-sm p-6">
                <div class="flex justify-between items-center mb-4">
                    <h3 class="text-lg font-semibold">👥 Lista de Funcionários</h3>
                    <select id="employeeFilterStatus" onchange="filterEmployees()" class="px-3 py-2 border border-gray-300 rounded-lg text-sm">
                        <option value="all">Todos</option>
                        <option value="ativo">Ativos</option>
                        <option value="ferias">Férias</option>
                        <option value="afastado">Afastados</option>
                        <option value="licenca">Licença</option>
                        <option value="demitido">Demitidos</option>
                    </select>
                </div>
                <div id="employeeList" class="space-y-3">
                    <p class="text-gray-500 text-sm">Nenhum funcionário cadastrado ainda</p>
                </div>
            </div>

            <!-- Production Records -->
            <div class="mt-6 bg-white rounded-xl shadow-sm p-6">
                <div class="flex justify-between items-center mb-4">
                    <h3 class="text-lg font-semibold">📊 Registros de Produção</h3>
                    <div class="flex space-x-2">
                        <select id="productionFilterEmployee" onchange="filterProductionRecords()" class="px-3 py-2 border border-gray-300 rounded-lg text-sm">
                            <option value="all">Todos os funcionários</option>
                        </select>
                        <select id="productionFilterPeriod" onchange="filterProductionRecords()" class="px-3 py-2 border border-gray-300 rounded-lg text-sm">
                            <option value="week">Última semana</option>
                            <option value="month">Último mês</option>
                            <option value="all">Todos os registros</option>
                        </select>
                    </div>
                </div>
                <div id="productionRecordsList" class="space-y-3">
                    <p class="text-gray-500 text-sm">Nenhum registro de produção ainda</p>
                </div>
            </div>

            <!-- Payroll History -->
            <div class="mt-6 bg-white rounded-xl shadow-sm p-6">
                <h3 class="text-lg font-semibold mb-4">💰 Histórico de Pagamentos</h3>
                <div id="payrollHistory" class="space-y-3">
                    <p class="text-gray-500 text-sm">Nenhum pagamento registrado ainda</p>
                </div>
            </div>
        </div>

        <!-- Settings Tab -->
        <div id="settings" class="tab-content hidden">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-6">
                <!-- Farm Settings -->
                <div class="bg-white rounded-xl shadow-sm p-6">
                    <h3 class="text-lg font-semibold mb-4">🏡 Configurações da Fazenda</h3>
                    <div class="space-y-4">
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Nome da fazenda</label>
                            <input type="text" id="farmNameInput" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent" placeholder="Ex: Fazenda São José">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Proprietário</label>
                            <input type="text" id="farmOwner" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent" placeholder="Ex: João Silva">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Localização</label>
                            <input type="text" id="farmLocation" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent" placeholder="Ex: Minas Gerais, Brasil">
                        </div>
                        <div class="grid grid-cols-2 gap-4">
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Área total (Alqueires)</label>
                                <input type="number" id="farmTotalArea" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent" placeholder="Ex: 50">
                            </div>
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Altitude (metros)</label>
                                <input type="number" id="farmAltitude" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent" placeholder="Ex: 800">
                            </div>
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Tipo de café principal</label>
                            <select id="farmMainCoffee" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent">
                                <option value="arabica">Arábica</option>
                                <option value="robusta">Robusta</option>
                                <option value="bourbon">Bourbon</option>
                                <option value="catuai">Catuaí</option>
                                <option value="mundo-novo">Mundo Novo</option>
                                <option value="acaia">Acaiá</option>
                                <option value="topazio">Topázio</option>
                            </select>
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Observações</label>
                            <textarea id="farmNotes" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent" rows="3" placeholder="Informações adicionais sobre a propriedade..."></textarea>
                        </div>
                        <button onclick="saveFarmSettings()" class="w-full bg-green-600 text-white py-3 rounded-lg hover:bg-green-700 transition-colors font-medium">
                            Salvar Configurações
                        </button>
                    </div>
                </div>

                <!-- System Settings -->
                <div class="bg-white rounded-xl shadow-sm p-6">
                    <h3 class="text-lg font-semibold mb-4">⚙️ Configurações do Sistema</h3>
                    <div class="space-y-4">
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Moeda padrão</label>
                            <select id="systemCurrency" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                                <option value="BRL">Real Brasileiro (R$)</option>
                                <option value="USD">Dólar Americano ($)</option>
                                <option value="EUR">Euro (€)</option>
                            </select>
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Unidade de área padrão</label>
                            <select id="systemAreaUnit" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                                <option value="alqueires">Alqueires Paulistas</option>
                                <option value="hectares">Hectares</option>
                                <option value="acres">Acres</option>
                            </select>
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Formato de data</label>
                            <select id="systemDateFormat" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                                <option value="DD/MM/YYYY">DD/MM/AAAA</option>
                                <option value="MM/DD/YYYY">MM/DD/AAAA</option>
                                <option value="YYYY-MM-DD">AAAA-MM-DD</option>
                            </select>
                        </div>
                        <div class="border-t pt-4">
                            <h4 class="font-medium mb-3">📊 Dados do Sistema</h4>
                            <div class="space-y-2 text-sm">
                                <div class="flex justify-between">
                                    <span>Tarefas cadastradas:</span>
                                    <span id="systemTaskCount">0</span>
                                </div>
                                <div class="flex justify-between">
                                    <span>Itens no estoque:</span>
                                    <span id="systemInventoryCount">0</span>
                                </div>
                                <div class="flex justify-between">
                                    <span>Equipamentos:</span>
                                    <span id="systemEquipmentCount">0</span>
                                </div>
                                <div class="flex justify-between">
                                    <span>Funcionários:</span>
                                    <span id="systemEmployeeCount">0</span>
                                </div>
                            </div>
                        </div>
                        <button onclick="saveSystemSettings()" class="w-full bg-blue-600 text-white py-3 rounded-lg hover:bg-blue-700 transition-colors font-medium">
                            Salvar Configurações
                        </button>
                    </div>
                </div>
            </div>

            <!-- Reminder Settings -->
            <div class="mt-6 bg-white rounded-xl shadow-sm p-6">
                <h3 class="text-lg font-semibold mb-4">🔔 Configurações de Lembretes</h3>
                <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                    <div class="space-y-3">
                        <h4 class="font-medium text-gray-700">Lembretes Financeiros</h4>
                        <label class="flex items-center space-x-2">
                            <input type="checkbox" id="payrollReminderSetting" checked class="rounded">
                            <span class="text-sm">💰 Pagamento de funcionários (todo dia 5)</span>
                        </label>
                        <label class="flex items-center space-x-2">
                            <input type="checkbox" id="contractReminderSetting" checked class="rounded">
                            <span class="text-sm">📄 Vencimento de contratos</span>
                        </label>
                        <label class="flex items-center space-x-2">
                            <input type="checkbox" id="vacationReminderSetting" checked class="rounded">
                            <span class="text-sm">🏖️ Período de férias dos funcionários</span>
                        </label>
                    </div>
                    <div class="space-y-3">
                        <h4 class="font-medium text-gray-700">Lembretes Operacionais</h4>
                        <label class="flex items-center space-x-2">
                            <input type="checkbox" id="taskReminderSetting" checked class="rounded">
                            <span class="text-sm">✅ Tarefas pendentes e atrasadas</span>
                        </label>
                        <label class="flex items-center space-x-2">
                            <input type="checkbox" id="maintenanceReminderSetting" checked class="rounded">
                            <span class="text-sm">🔧 Manutenção de equipamentos</span>
                        </label>
                        <label class="flex items-center space-x-2">
                            <input type="checkbox" id="stockReminderSetting" checked class="rounded">
                            <span class="text-sm">📦 Estoque baixo</span>
                        </label>
                    </div>
                    <div class="space-y-3">
                        <h4 class="font-medium text-gray-700">Lembretes Agrícolas</h4>
                        <label class="flex items-center space-x-2">
                            <input type="checkbox" id="harvestReminderSetting" checked class="rounded">
                            <span class="text-sm">☕ Época de colheita</span>
                        </label>
                        <label class="flex items-center space-x-2">
                            <input type="checkbox" id="irrigationReminderSetting" checked class="rounded">
                            <span class="text-sm">💧 Cronograma de irrigação</span>
                        </label>
                        <label class="flex items-center space-x-2">
                            <input type="checkbox" id="fertilizerReminderSetting" checked class="rounded">
                            <span class="text-sm">🌱 Cronograma de adubação</span>
                        </label>
                    </div>
                    <div class="flex items-end">
                        <button onclick="saveReminderSettings()" class="w-full bg-blue-600 text-white py-3 rounded-lg hover:bg-blue-700 transition-colors font-medium">
                            Salvar Configurações de Lembretes
                        </button>
                    </div>
                </div>
            </div>

            <!-- Data Management -->
            <div class="mt-6 bg-white rounded-xl shadow-sm p-6">
                <h3 class="text-lg font-semibold mb-4">💾 Gerenciamento de Dados</h3>
                <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
                    <button onclick="exportData()" class="bg-green-600 text-white py-3 px-4 rounded-lg hover:bg-green-700 transition-colors font-medium">
                        📤 Exportar Dados
                    </button>
                    <button onclick="importData()" class="bg-blue-600 text-white py-3 px-4 rounded-lg hover:bg-blue-700 transition-colors font-medium">
                        📥 Importar Dados
                    </button>
                    <button onclick="clearAllData()" class="bg-red-600 text-white py-3 px-4 rounded-lg hover:bg-red-700 transition-colors font-medium">
                        🗑️ Limpar Todos os Dados
                    </button>
                </div>
                <p class="text-sm text-gray-600 mt-4">
                    ⚠️ Atenção: As operações de importação e limpeza de dados são irreversíveis. 
                    Recomendamos fazer backup dos dados antes de prosseguir.
                </p>
            </div>
        </div>

        <!-- Calculator Tab -->
        <div id="calculator" class="tab-content hidden">
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- Unit Converter -->
                <div class="bg-white rounded-xl shadow-sm p-6">
                    <h3 class="text-lg font-semibold mb-4">🔄 Conversor de Unidades</h3>
                    <div class="space-y-4">
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Hectares</label>
                            <input type="number" id="hectares" onchange="convertUnits()" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="0">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Alqueires Paulistas</label>
                            <input type="number" id="alqueires" onchange="convertFromAlqueires()" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="0">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Metros Quadrados</label>
                            <input type="number" id="squareMeters" readonly class="w-full p-3 border border-gray-300 rounded-lg bg-gray-50" placeholder="0">
                        </div>
                    </div>
                </div>

                <!-- Productivity Calculator -->
                <div class="bg-white rounded-xl shadow-sm p-6">
                    <h3 class="text-lg font-semibold mb-4">📈 Calculadora de Produtividade</h3>
                    <div class="space-y-4">
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Produção (sacas)</label>
                            <input type="number" id="production" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent" placeholder="Ex: 1500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Área (Alqueires)</label>
                            <input type="number" id="productivityArea" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent" placeholder="Ex: 10">
                        </div>
                        <button onclick="calculateProductivity()" class="w-full bg-green-600 text-white py-3 rounded-lg hover:bg-green-700 transition-colors font-medium">
                            Calcular Produtividade
                        </button>
                        <div id="productivityResult" class="hidden bg-green-50 p-4 rounded-lg">
                            <p class="text-sm text-gray-600">Produtividade:</p>
                            <p class="text-lg font-semibold text-green-600" id="productivityValue"></p>
                        </div>
                    </div>
                </div>

                <!-- Cost per Bag Calculator -->
                <div class="bg-white rounded-xl shadow-sm p-6">
                    <h3 class="text-lg font-semibold mb-4">💰 Custo por Saca</h3>
                    <div class="space-y-4">
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Custo total (R$)</label>
                            <input type="number" id="totalCost" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-purple-500 focus:border-transparent" placeholder="Ex: 50000">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Produção (sacas)</label>
                            <input type="number" id="totalProduction" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-purple-500 focus:border-transparent" placeholder="Ex: 1500">
                        </div>
                        <button onclick="calculateCostPerBag()" class="w-full bg-purple-600 text-white py-3 rounded-lg hover:bg-purple-700 transition-colors font-medium">
                            Calcular Custo
                        </button>
                        <div id="costPerBagResult" class="hidden bg-purple-50 p-4 rounded-lg">
                            <p class="text-sm text-gray-600">Custo por saca:</p>
                            <p class="text-lg font-semibold text-purple-600" id="costPerBagValue"></p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </main>

    <script>
        // Global variables
        let currentTab = 'dashboard';
        let plantingRecords = [];
        let irrigationSchedules = [];
        let fertilizerSchedules = [];
        let revenues = [];
        let expenses = [];
        let tasks = [];
        let inventory = [];
        let equipment = [];
        let harvestRecords = [];
        let employees = [];
        let payrollRecords = [];
        let productionRecords = [];
        let farmSettings = {
            name: 'Minha Propriedade',
            owner: '',
            location: '',
            totalArea: 0,
            altitude: 0,
            mainCoffee: 'arabica',
            notes: ''
        };
        let reminders = [];
        let reminderSettings = {
            payrollReminder: true,
            taskReminder: true,
            maintenanceReminder: true,
            stockReminder: true,
            harvestReminder: true,
            irrigationReminder: true,
            fertilizerReminder: true,
            contractReminder: true,
            vacationReminder: true
        };

        // PWA Installation
        let deferredPrompt;
        let isInstallable = false;

        // Service Worker Registration
        if ('serviceWorker' in navigator) {
            window.addEventListener('load', function() {
                const swCode = `
                    const CACHE_NAME = 'cafeplan-pro-v1';
                    const urlsToCache = [
                        './',
                        'https://cdn.tailwindcss.com'
                    ];

                    self.addEventListener('install', function(event) {
                        event.waitUntil(
                            caches.open(CACHE_NAME)
                                .then(function(cache) {
                                    return cache.addAll(urlsToCache);
                                })
                        );
                    });

                    self.addEventListener('fetch', function(event) {
                        event.respondWith(
                            caches.match(event.request)
                                .then(function(response) {
                                    if (response) {
                                        return response;
                                    }
                                    return fetch(event.request);
                                }
                            )
                        );
                    });
                `;
                
                const blob = new Blob([swCode], { type: 'application/javascript' });
                const swUrl = URL.createObjectURL(blob);
                
                navigator.serviceWorker.register(swUrl)
                    .then(function(registration) {
                        console.log('ServiceWorker registration successful');
                    })
                    .catch(function(err) {
                        console.log('ServiceWorker registration failed: ', err);
                    });
            });
        }

        // PWA Install Prompt
        window.addEventListener('beforeinstallprompt', (e) => {
            e.preventDefault();
            deferredPrompt = e;
            isInstallable = true;
            showInstallOptions();
        });

        function showInstallOptions() {
            // Show banner
            document.getElementById('installBanner').classList.remove('hidden');
            
            // Show header button
            document.getElementById('installButtonHeader').classList.remove('hidden');
        }

        function hideInstallOptions() {
            // Hide banner
            document.getElementById('installBanner').classList.add('hidden');
            
            // Hide header button
            document.getElementById('installButtonHeader').classList.add('hidden');
        }

        function installPWA() {
            if (deferredPrompt) {
                deferredPrompt.prompt();
                deferredPrompt.userChoice.then((choiceResult) => {
                    if (choiceResult.outcome === 'accepted') {
                        console.log('User accepted the install prompt');
                        hideInstallOptions();
                        showInstallSuccessMessage();
                    }
                    deferredPrompt = null;
                });
            } else {
                // Fallback for browsers that don't support PWA installation
                showManualInstallInstructions();
            }
        }

        function dismissInstallBanner() {
            document.getElementById('installBanner').classList.add('hidden');
            // Keep header button visible
        }

        function showInstallSuccessMessage() {
            alert('🎉 CaféPlan Pro foi instalado com sucesso!\n\nVocê pode encontrar o app na tela inicial do seu dispositivo.');
        }

        function showManualInstallInstructions() {
            const isIOS = /iPad|iPhone|iPod/.test(navigator.userAgent);
            const isAndroid = /Android/.test(navigator.userAgent);
            
            let instructions = '📱 Como Instalar o CaféPlan Pro:\n\n';
            
            if (isIOS) {
                instructions += '🍎 No iPhone/iPad (Safari):\n';
                instructions += '1. Toque no botão de compartilhar (□↗)\n';
                instructions += '2. Role para baixo e toque em "Adicionar à Tela de Início"\n';
                instructions += '3. Toque em "Adicionar"\n';
                instructions += '4. O app aparecerá na sua tela inicial!';
            } else if (isAndroid) {
                instructions += '🤖 No Android (Chrome):\n';
                instructions += '1. Toque no menu (⋮) do navegador\n';
                instructions += '2. Selecione "Adicionar à tela inicial"\n';
                instructions += '3. Toque em "Adicionar"\n';
                instructions += '4. O app aparecerá na sua tela inicial!';
            } else {
                instructions += '💻 No seu navegador:\n';
                instructions += '1. Procure pelo ícone de instalação na barra de endereços\n';
                instructions += '2. Ou use o menu do navegador\n';
                instructions += '3. Selecione "Instalar aplicativo" ou "Adicionar à tela inicial"\n';
                instructions += '4. Siga as instruções na tela';
            }
            
            instructions += '\n\n✨ Após instalar, você poderá usar o app offline e com acesso rápido!';
            
            alert(instructions);
        }

        // Hide install options if already installed
        window.addEventListener('appinstalled', (evt) => {
            hideInstallOptions();
            showInstallSuccessMessage();
        });

        // Check if app is already installed (running in standalone mode)
        if (window.matchMedia('(display-mode: standalone)').matches || window.navigator.standalone) {
            // App is already installed, hide install options
            hideInstallOptions();
        } else {
            // Show install options after a short delay if not installable via prompt
            setTimeout(() => {
                if (!isInstallable) {
                    showInstallOptions();
                }
            }, 3000);
        }

        // Initialize app
        document.addEventListener('DOMContentLoaded', function() {
            updateDateTime();
            setInterval(updateDateTime, 60000); // Update every minute
            
            // Set today's date as default for date inputs
            const today = new Date().toISOString().split('T')[0];
            document.getElementById('revenueDate').value = today;
            document.getElementById('expenseDate').value = today;
            document.getElementById('fertilizerDate').value = today;
            document.getElementById('taskDate').value = today;
            document.getElementById('harvestDate').value = today;
            document.getElementById('productionDate').value = today;
            document.getElementById('accumulatedPaymentDate').value = today;
            
            // Set report dates to current month
            const firstDay = new Date(new Date().getFullYear(), new Date().getMonth(), 1).toISOString().split('T')[0];
            document.getElementById('reportStartDate').value = firstDay;
            document.getElementById('reportEndDate').value = today;
            document.getElementById('payrollDate').value = today;
            
            // Initialize weather forecast
            generateWeatherForecast();
            
            // Initialize financial summary
            updateFinancialSummary();
            updateDashboard();
            
            // Load farm settings
            loadFarmSettings();
            
            // Initialize reminders
            generateReminders();
            updateReminders();
            
            // Initialize production tracking
            updateProductionSummary();
            updateProductionEmployeeSelects();
            renderProductionRecords();
            
            // Update reminders every hour
            setInterval(updateReminders, 3600000);
            
            // Load saved data from localStorage
            loadDataFromStorage();
            
            // Auto-save data every 30 seconds
            setInterval(saveDataToStorage, 30000);
            
            // Save data when page is about to unload
            window.addEventListener('beforeunload', saveDataToStorage);
        });

        // Data persistence functions
        function saveDataToStorage() {
            try {
                const data = {
                    farmSettings: farmSettings,
                    employees: employees,
                    payrollRecords: payrollRecords,
                    productionRecords: productionRecords,
                    tasks: tasks,
                    inventory: inventory,
                    equipment: equipment,
                    revenues: revenues,
                    expenses: expenses,
                    harvestRecords: harvestRecords,
                    plantingRecords: plantingRecords,
                    irrigationSchedules: irrigationSchedules,
                    fertilizerSchedules: fertilizerSchedules,
                    reminderSettings: reminderSettings,
                    lastSaved: new Date().toISOString()
                };
                
                localStorage.setItem('cafeplan-data', JSON.stringify(data));
                console.log('Data saved to localStorage');
            } catch (error) {
                console.error('Error saving data to localStorage:', error);
            }
        }

        function loadDataFromStorage() {
            try {
                const savedData = localStorage.getItem('cafeplan-data');
                if (savedData) {
                    const data = JSON.parse(savedData);
                    
                    // Load all data
                    if (data.farmSettings) farmSettings = data.farmSettings;
                    if (data.employees) employees = data.employees;
                    if (data.payrollRecords) payrollRecords = data.payrollRecords;
                    if (data.productionRecords) productionRecords = data.productionRecords;
                    if (data.tasks) tasks = data.tasks;
                    if (data.inventory) inventory = data.inventory;
                    if (data.equipment) equipment = data.equipment;
                    if (data.revenues) revenues = data.revenues;
                    if (data.expenses) expenses = data.expenses;
                    if (data.harvestRecords) harvestRecords = data.harvestRecords;
                    if (data.plantingRecords) plantingRecords = data.plantingRecords;
                    if (data.irrigationSchedules) irrigationSchedules = data.irrigationSchedules;
                    if (data.fertilizerSchedules) fertilizerSchedules = data.fertilizerSchedules;
                    if (data.reminderSettings) reminderSettings = data.reminderSettings;
                    
                    console.log('Data loaded from localStorage');
                    
                    // Refresh displays after loading
                    setTimeout(() => {
                        loadFarmSettings();
                        renderEmployees();
                        renderPayrollHistory();
                        renderProductionRecords();
                        updateEmployeeSummary();
                        updatePayrollEmployeeSelect();
                        updateProductionEmployeeSelects();
                        updateProductionSummary();
                        renderTasks();
                        renderInventory();
                        renderEquipment();
                        updateFinancialSummary();
                        updateDashboard();
                        updateReminders();
                        renderPlantingRecords();
                        renderIrrigationSchedule();
                        renderFertilizerSchedule();
                        renderHarvestRecords();
                        updateHarvestSummary();
                        updateInventorySummary();
                        updateEquipmentSummary();
                        updateSystemStats();
                    }, 100);
                }
            } catch (error) {
                console.error('Error loading data from localStorage:', error);
            }
        }

        function updateDateTime() {
            const now = new Date();
            const options = { 
                weekday: 'long', 
                year: 'numeric', 
                month: 'long', 
                day: 'numeric',
                hour: '2-digit',
                minute: '2-digit'
            };
            document.getElementById('currentDateTime').textContent = now.toLocaleDateString('pt-BR', options);
        }

        // Tab management
        function showTab(tabName) {
            // Hide all tabs
            document.querySelectorAll('.tab-content').forEach(tab => {
                tab.classList.add('hidden');
            });
            
            // Remove active class from all buttons
            document.querySelectorAll('.tab-btn').forEach(btn => {
                btn.classList.remove('tab-active');
                btn.classList.add('text-gray-600', 'hover:text-gray-800');
            });
            
            // Show selected tab
            document.getElementById(tabName).classList.remove('hidden');
            
            // Find and activate the correct button
            const activeButton = document.querySelector(`button[onclick="showTab('${tabName}')"]`);
            if (activeButton) {
                activeButton.classList.add('tab-active');
                activeButton.classList.remove('text-gray-600', 'hover:text-gray-800');
            }
            
            currentTab = tabName;
        }

        // Area calculations
        function calculateArea() {
            const length = parseFloat(document.getElementById('length').value);
            const width = parseFloat(document.getElementById('width').value);
            
            if (!length || !width) {
                alert('Por favor, preencha comprimento e largura');
                return;
            }
            
            const areaM2 = length * width;
            const areaAlqueires = areaM2 / 24200; // 1 alqueire paulista = 24.200 m²
            const areaHectares = areaM2 / 10000;
            
            document.getElementById('areaValue').textContent = `${areaAlqueires.toFixed(2)} Alqueires Paulistas`;
            document.getElementById('areaHectares').textContent = `${areaHectares.toFixed(2)} hectares | ${areaM2.toLocaleString()} m²`;
            document.getElementById('areaResult').classList.remove('hidden');
            
            // Update dashboard
            document.getElementById('totalArea').textContent = areaAlqueires.toFixed(2);
        }

        // Planting calculations
        function calculatePlanting() {
            const area = parseFloat(document.getElementById('plantingArea').value);
            const rowSpacing = parseFloat(document.getElementById('rowSpacing').value);
            const plantSpacing = parseFloat(document.getElementById('plantSpacing').value);
            
            if (!area || !rowSpacing || !plantSpacing) {
                alert('Por favor, preencha todos os campos');
                return;
            }
            
            const areaM2 = area * 24200; // Convert alqueires to m²
            const plantsPerM2 = 1 / (rowSpacing * plantSpacing);
            const totalPlants = Math.round(areaM2 * plantsPerM2);
            const density = Math.round(plantsPerM2 * 10000); // Plants per hectare
            
            document.getElementById('seedlingsNeeded').textContent = `${totalPlants.toLocaleString()} mudas`;
            document.getElementById('plantingDensity').textContent = `Densidade: ${density.toLocaleString()} plantas/hectare`;
            document.getElementById('plantingResult').classList.remove('hidden');
            
            // Update dashboard
            document.getElementById('totalPlants').textContent = totalPlants.toLocaleString();
        }

        // Add planting record
        function addPlantingRecord() {
            const area = document.getElementById('plantingArea').value;
            const variety = document.getElementById('coffeeVariety').value;
            const seedlings = document.getElementById('seedlingsNeeded').textContent;
            
            if (!area || !seedlings || seedlings === '') {
                alert('Primeiro calcule as mudas necessárias');
                return;
            }
            
            const record = {
                id: Date.now(),
                date: new Date().toLocaleDateString('pt-BR'),
                area: area,
                variety: variety,
                seedlings: seedlings,
                rowSpacing: document.getElementById('rowSpacing').value,
                plantSpacing: document.getElementById('plantSpacing').value
            };
            
            plantingRecords.push(record);
            renderPlantingRecords();
            saveDataToStorage();
        }

        function renderPlantingRecords() {
            const container = document.getElementById('plantingRecords');
            container.innerHTML = '';
            
            if (plantingRecords.length === 0) {
                container.innerHTML = '<p class="text-gray-500 text-sm">Nenhum plantio registrado ainda</p>';
                return;
            }
            
            plantingRecords.forEach(record => {
                const div = document.createElement('div');
                div.className = 'bg-gray-50 p-4 rounded-lg flex justify-between items-center';
                div.innerHTML = `
                    <div>
                        <p class="font-medium">${record.area} Alqueires - ${record.variety} - ${record.seedlings}</p>
                        <p class="text-sm text-gray-600">Espaçamento: ${record.rowSpacing}m x ${record.plantSpacing}m | ${record.date}</p>
                    </div>
                    <button onclick="removePlantingRecord(${record.id})" class="text-red-600 hover:text-red-800">
                        <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                            <path d="M19 6.41L17.59 5 12 10.59 6.41 5 5 6.41 10.59 12 5 17.59 6.41 19 12 13.41 17.59 19 19 17.59 13.41 12z"/>
                        </svg>
                    </button>
                `;
                container.appendChild(div);
            });
        }

        function removePlantingRecord(id) {
            plantingRecords = plantingRecords.filter(record => record.id !== id);
            renderPlantingRecords();
        }

        // Irrigation calculations
        function calculateIrrigation() {
            const area = parseFloat(document.getElementById('irrigationArea').value);
            const waterDepth = parseFloat(document.getElementById('waterDepth').value);
            const efficiency = parseFloat(document.getElementById('efficiency').value);
            
            if (!area || !waterDepth || !efficiency) {
                alert('Por favor, preencha todos os campos');
                return;
            }
            
            const areaM2 = area * 24200; // Convert alqueires to m²
            const waterNeeded = (areaM2 * waterDepth) / 1000; // m³
            const waterWithEfficiency = waterNeeded / (efficiency / 100);
            
            document.getElementById('waterVolume').textContent = `${waterWithEfficiency.toFixed(0)} m³/dia`;
            document.getElementById('irrigationTime').textContent = `Eficiência: ${efficiency}% | ${waterNeeded.toFixed(0)} m³ líquidos`;
            document.getElementById('irrigationResult').classList.remove('hidden');
        }

        function addIrrigationSchedule() {
            const sector = document.getElementById('irrigationSector').value;
            const time = document.getElementById('irrigationTimeSchedule').value;
            const duration = document.getElementById('irrigationDuration').value;
            
            if (!sector || !time || !duration) {
                alert('Por favor, preencha todos os campos');
                return;
            }
            
            const schedule = {
                id: Date.now(),
                sector: sector,
                time: time,
                duration: duration,
                date: new Date().toLocaleDateString('pt-BR')
            };
            
            irrigationSchedules.push(schedule);
            renderIrrigationSchedule();
            
            // Clear form
            document.getElementById('irrigationSector').value = '';
            document.getElementById('irrigationTimeSchedule').value = '';
            document.getElementById('irrigationDuration').value = '';
        }

        function renderIrrigationSchedule() {
            const container = document.getElementById('irrigationSchedule');
            container.innerHTML = '';
            
            if (irrigationSchedules.length === 0) {
                container.innerHTML = '<p class="text-gray-500 text-sm">Nenhuma irrigação agendada</p>';
                return;
            }
            
            irrigationSchedules.forEach(schedule => {
                const div = document.createElement('div');
                div.className = 'bg-blue-50 p-3 rounded-lg flex justify-between items-center';
                div.innerHTML = `
                    <div>
                        <p class="font-medium">${schedule.sector} - ${schedule.time}</p>
                        <p class="text-sm text-gray-600">${schedule.duration}h de duração</p>
                    </div>
                    <button onclick="removeIrrigationSchedule(${schedule.id})" class="text-red-600 hover:text-red-800">
                        <svg class="w-4 h-4" fill="currentColor" viewBox="0 0 24 24">
                            <path d="M19 6.41L17.59 5 12 10.59 6.41 5 5 6.41 10.59 12 5 17.59 6.41 19 12 13.41 17.59 19 19 17.59 13.41 12z"/>
                        </svg>
                    </button>
                `;
                container.appendChild(div);
            });
        }

        function removeIrrigationSchedule(id) {
            irrigationSchedules = irrigationSchedules.filter(schedule => schedule.id !== id);
            renderIrrigationSchedule();
        }

        // Fertilizer calculations
        function calculateFertilizer() {
            const area = parseFloat(document.getElementById('fertilizerArea').value);
            const dose = parseFloat(document.getElementById('fertilizerDose').value);
            
            if (!area || !dose) {
                alert('Por favor, preencha área e dosagem');
                return;
            }
            
            const totalAmount = area * dose;
            const estimatedCost = totalAmount * 3.5; // Estimated cost per kg
            
            document.getElementById('fertilizerAmount').textContent = `${totalAmount.toFixed(0)} kg`;
            document.getElementById('fertilizerCost').textContent = `Custo estimado: R$ ${estimatedCost.toLocaleString('pt-BR', {minimumFractionDigits: 2})}`;
            document.getElementById('fertilizerResult').classList.remove('hidden');
        }

        function addFertilizerSchedule() {
            const date = document.getElementById('fertilizerDate').value;
            const sector = document.getElementById('fertilizerSector').value;
            const notes = document.getElementById('fertilizerNotes').value;
            
            if (!date || !sector) {
                alert('Por favor, preencha data e setor');
                return;
            }
            
            const schedule = {
                id: Date.now(),
                date: new Date(date).toLocaleDateString('pt-BR'),
                sector: sector,
                notes: notes
            };
            
            fertilizerSchedules.push(schedule);
            renderFertilizerSchedule();
            
            // Clear form
            document.getElementById('fertilizerSector').value = '';
            document.getElementById('fertilizerNotes').value = '';
        }

        function renderFertilizerSchedule() {
            const container = document.getElementById('fertilizerSchedule');
            container.innerHTML = '';
            
            if (fertilizerSchedules.length === 0) {
                container.innerHTML = '<p class="text-gray-500 text-sm">Nenhuma adubação agendada</p>';
                return;
            }
            
            fertilizerSchedules.forEach(schedule => {
                const div = document.createElement('div');
                div.className = 'bg-green-50 p-3 rounded-lg flex justify-between items-center';
                div.innerHTML = `
                    <div>
                        <p class="font-medium">${schedule.sector} - ${schedule.date}</p>
                        ${schedule.notes ? `<p class="text-sm text-gray-600">${schedule.notes}</p>` : ''}
                    </div>
                    <button onclick="removeFertilizerSchedule(${schedule.id})" class="text-red-600 hover:text-red-800">
                        <svg class="w-4 h-4" fill="currentColor" viewBox="0 0 24 24">
                            <path d="M19 6.41L17.59 5 12 10.59 6.41 5 5 6.41 10.59 12 5 17.59 6.41 19 12 13.41 17.59 19 19 17.59 13.41 12z"/>
                        </svg>
                    </button>
                `;
                container.appendChild(div);
            });
        }

        function removeFertilizerSchedule(id) {
            fertilizerSchedules = fertilizerSchedules.filter(schedule => schedule.id !== id);
            renderFertilizerSchedule();
        }

        // Financial management
        function addRevenue() {
            const description = document.getElementById('revenueDescription').value;
            const amount = parseFloat(document.getElementById('revenueAmount').value);
            const date = document.getElementById('revenueDate').value;
            
            if (!description || !amount || !date) {
                alert('Por favor, preencha todos os campos');
                return;
            }
            
            const revenue = {
                id: Date.now(),
                type: 'revenue',
                description: description,
                amount: amount,
                date: new Date(date).toLocaleDateString('pt-BR')
            };
            
            revenues.push(revenue);
            updateFinancialSummary();
            updateDashboard();
            
            // Clear form
            document.getElementById('revenueDescription').value = '';
            document.getElementById('revenueAmount').value = '';
        }

        function addExpense() {
            const description = document.getElementById('expenseDescription').value;
            const amount = parseFloat(document.getElementById('expenseAmount').value);
            const category = document.getElementById('expenseCategory').value;
            const date = document.getElementById('expenseDate').value;
            
            if (!description || !amount || !date) {
                alert('Por favor, preencha todos os campos');
                return;
            }
            
            const expense = {
                id: Date.now(),
                type: 'expense',
                description: description,
                amount: amount,
                category: category,
                date: new Date(date).toLocaleDateString('pt-BR')
            };
            
            expenses.push(expense);
            updateFinancialSummary();
            updateDashboard();
            
            // Clear form
            document.getElementById('expenseDescription').value = '';
            document.getElementById('expenseAmount').value = '';
        }

        function updateFinancialSummary() {
            const totalRevenue = revenues.reduce((sum, r) => sum + r.amount, 0);
            const totalExpenses = expenses.reduce((sum, e) => sum + e.amount, 0);
            const netProfit = totalRevenue - totalExpenses;
            
            document.getElementById('totalRevenue').textContent = `R$ ${totalRevenue.toLocaleString('pt-BR', {minimumFractionDigits: 2})}`;
            document.getElementById('totalExpenses').textContent = `R$ ${totalExpenses.toLocaleString('pt-BR', {minimumFractionDigits: 2})}`;
            document.getElementById('netProfit').textContent = `R$ ${netProfit.toLocaleString('pt-BR', {minimumFractionDigits: 2})}`;
            
            // Update monthly revenue in dashboard
            document.getElementById('monthlyRevenue').textContent = `R$ ${totalRevenue.toLocaleString('pt-BR')}`;
            
            // Render financial records
            renderFinancialRecords();
        }

        function renderFinancialRecords() {
            const container = document.getElementById('financialRecords');
            container.innerHTML = '';
            
            const allRecords = [...revenues, ...expenses].sort((a, b) => new Date(b.date.split('/').reverse().join('-')) - new Date(a.date.split('/').reverse().join('-')));
            
            if (allRecords.length === 0) {
                container.innerHTML = '<p class="text-gray-500 text-sm">Nenhuma movimentação financeira registrada</p>';
                return;
            }
            
            allRecords.slice(0, 10).forEach(record => {
                const div = document.createElement('div');
                const isRevenue = record.type === 'revenue';
                div.className = `flex justify-between items-center p-3 rounded-lg ${isRevenue ? 'bg-green-50' : 'bg-red-50'}`;
                div.innerHTML = `
                    <div>
                        <p class="font-medium">${record.description}</p>
                        <p class="text-sm text-gray-600">${record.date}${record.category ? ` | ${record.category}` : ''}</p>
                    </div>
                    <p class="font-bold ${isRevenue ? 'text-green-600' : 'text-red-600'}">
                        ${isRevenue ? '+' : '-'} R$ ${record.amount.toLocaleString('pt-BR', {minimumFractionDigits: 2})}
                    </p>
                `;
                container.appendChild(div);
            });
        }

        // Task management
        function addTask() {
            const title = document.getElementById('taskTitle').value;
            const category = document.getElementById('taskCategory').value;
            const priority = document.getElementById('taskPriority').value;
            const date = document.getElementById('taskDate').value;
            const responsible = document.getElementById('taskResponsible').value;
            const notes = document.getElementById('taskNotes').value;
            
            if (!title || !date) {
                alert('Por favor, preencha título e data');
                return;
            }
            
            const task = {
                id: Date.now(),
                title: title,
                category: category,
                priority: priority,
                date: date,
                responsible: responsible,
                notes: notes,
                completed: false,
                createdAt: new Date().toISOString()
            };
            
            tasks.push(task);
            renderTasks();
            updateDashboard();
            
            // Clear form
            document.getElementById('taskTitle').value = '';
            document.getElementById('taskResponsible').value = '';
            document.getElementById('taskNotes').value = '';
        }

        function renderTasks() {
            const container = document.getElementById('taskList');
            container.innerHTML = '';
            
            const filteredTasks = filterTasksArray();
            
            if (filteredTasks.length === 0) {
                container.innerHTML = '<p class="text-gray-500 text-sm">Nenhuma tarefa encontrada</p>';
                return;
            }
            
            filteredTasks.forEach(task => {
                const div = document.createElement('div');
                const isOverdue = new Date(task.date) < new Date() && !task.completed;
                const priorityClass = `task-priority-${task.priority}`;
                
                div.className = `bg-white p-4 rounded-lg border ${priorityClass} ${task.completed ? 'opacity-60' : ''}`;
                div.innerHTML = `
                    <div class="flex items-start justify-between">
                        <div class="flex-1">
                            <div class="flex items-center space-x-2 mb-2">
                                <input type="checkbox" ${task.completed ? 'checked' : ''} onchange="toggleTask(${task.id})" class="rounded">
                                <h4 class="font-medium ${task.completed ? 'line-through' : ''}">${task.title}</h4>
                                <span class="px-2 py-1 text-xs rounded-full bg-gray-100">${task.category}</span>
                                ${isOverdue ? '<span class="px-2 py-1 text-xs rounded-full bg-red-100 text-red-800">Atrasada</span>' : ''}
                            </div>
                            <p class="text-sm text-gray-600">📅 ${new Date(task.date).toLocaleDateString('pt-BR')}</p>
                            ${task.responsible ? `<p class="text-sm text-gray-600">👤 ${task.responsible}</p>` : ''}
                            ${task.notes ? `<p class="text-sm text-gray-500 mt-1">${task.notes}</p>` : ''}
                        </div>
                        <button onclick="removeTask(${task.id})" class="text-red-600 hover:text-red-800 ml-2">
                            <svg class="w-4 h-4" fill="currentColor" viewBox="0 0 24 24">
                                <path d="M19 6.41L17.59 5 12 10.59 6.41 5 5 6.41 10.59 12 5 17.59 6.41 19 12 13.41 17.59 19 19 17.59 13.41 12z"/>
                            </svg>
                        </button>
                    </div>
                `;
                container.appendChild(div);
            });
        }

        function filterTasksArray() {
            const statusFilter = document.getElementById('taskFilter').value;
            const categoryFilter = document.getElementById('categoryFilter').value;
            
            return tasks.filter(task => {
                const statusMatch = statusFilter === 'all' || 
                    (statusFilter === 'pending' && !task.completed) ||
                    (statusFilter === 'completed' && task.completed) ||
                    (statusFilter === 'overdue' && new Date(task.date) < new Date() && !task.completed);
                
                const categoryMatch = categoryFilter === 'all' || task.category === categoryFilter;
                
                return statusMatch && categoryMatch;
            });
        }

        function filterTasks() {
            renderTasks();
        }

        function toggleTask(id) {
            const task = tasks.find(t => t.id === id);
            if (task) {
                task.completed = !task.completed;
                renderTasks();
                updateDashboard();
            }
        }

        function removeTask(id) {
            tasks = tasks.filter(task => task.id !== id);
            renderTasks();
            updateDashboard();
        }

        // Inventory management
        function addInventoryItem() {
            const name = document.getElementById('inventoryName').value;
            const category = document.getElementById('inventoryCategory').value;
            const quantity = parseFloat(document.getElementById('inventoryQuantity').value);
            const unit = document.getElementById('inventoryUnit').value;
            const price = parseFloat(document.getElementById('inventoryPrice').value);
            const minStock = parseFloat(document.getElementById('inventoryMinStock').value);
            const supplier = document.getElementById('inventorySupplier').value;
            
            if (!name || !quantity || !price) {
                alert('Por favor, preencha nome, quantidade e preço');
                return;
            }
            
            const item = {
                id: Date.now(),
                name: name,
                category: category,
                quantity: quantity,
                unit: unit,
                price: price,
                minStock: minStock || 0,
                supplier: supplier,
                addedAt: new Date().toISOString()
            };
            
            inventory.push(item);
            renderInventory();
            updateInventorySummary();
            
            // Clear form
            document.getElementById('inventoryName').value = '';
            document.getElementById('inventoryQuantity').value = '';
            document.getElementById('inventoryPrice').value = '';
            document.getElementById('inventoryMinStock').value = '';
            document.getElementById('inventorySupplier').value = '';
        }

        function renderInventory() {
            const container = document.getElementById('inventoryList');
            container.innerHTML = '';
            
            const filteredInventory = filterInventoryArray();
            
            if (filteredInventory.length === 0) {
                container.innerHTML = '<p class="text-gray-500 text-sm">Nenhum item encontrado</p>';
                return;
            }
            
            filteredInventory.forEach(item => {
                const div = document.createElement('div');
                const isLowStock = item.quantity <= item.minStock;
                
                div.className = `bg-white p-4 rounded-lg border ${isLowStock ? 'border-red-200 bg-red-50' : 'border-gray-200'}`;
                div.innerHTML = `
                    <div class="flex justify-between items-start">
                        <div class="flex-1">
                            <h4 class="font-medium">${item.name}</h4>
                            <p class="text-sm text-gray-600">${item.category} | ${item.supplier || 'Sem fornecedor'}</p>
                            <div class="flex items-center space-x-4 mt-2">
                                <span class="text-lg font-semibold ${isLowStock ? 'text-red-600' : 'text-green-600'}">${item.quantity} ${item.unit}</span>
                                <span class="text-sm text-gray-500">R$ ${item.price.toFixed(2)}/${item.unit}</span>
                                ${isLowStock ? '<span class="text-xs bg-red-100 text-red-800 px-2 py-1 rounded-full">Estoque baixo</span>' : ''}
                            </div>
                        </div>
                        <div class="flex space-x-2">
                            <button onclick="updateInventoryQuantity(${item.id}, 'add')" class="text-green-600 hover:text-green-800">
                                <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                                    <path d="M19 13h-6v6h-2v-6H5v-2h6V5h2v6h6v2z"/>
                                </svg>
                            </button>
                            <button onclick="updateInventoryQuantity(${item.id}, 'subtract')" class="text-yellow-600 hover:text-yellow-800">
                                <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                                    <path d="M19 13H5v-2h14v2z"/>
                                </svg>
                            </button>
                            <button onclick="removeInventoryItem(${item.id})" class="text-red-600 hover:text-red-800">
                                <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                                    <path d="M19 6.41L17.59 5 12 10.59 6.41 5 5 6.41 10.59 12 5 17.59 6.41 19 12 13.41 17.59 19 19 17.59 13.41 12z"/>
                                </svg>
                            </button>
                        </div>
                    </div>
                `;
                container.appendChild(div);
            });
        }

        function filterInventoryArray() {
            const categoryFilter = document.getElementById('inventoryFilterCategory').value;
            
            return inventory.filter(item => {
                return categoryFilter === 'all' || item.category === categoryFilter;
            });
        }

        function filterInventory() {
            renderInventory();
        }

        function updateInventoryQuantity(id, action) {
            const item = inventory.find(i => i.id === id);
            if (item) {
                const amount = parseFloat(prompt(`Quantidade a ${action === 'add' ? 'adicionar' : 'subtrair'}:`));
                if (amount && amount > 0) {
                    if (action === 'add') {
                        item.quantity += amount;
                    } else {
                        item.quantity = Math.max(0, item.quantity - amount);
                    }
                    renderInventory();
                    updateInventorySummary();
                }
            }
        }

        function removeInventoryItem(id) {
            inventory = inventory.filter(item => item.id !== id);
            renderInventory();
            updateInventorySummary();
        }

        function updateInventorySummary() {
            const totalItems = inventory.length;
            const lowStockItems = inventory.filter(item => item.quantity <= item.minStock).length;
            
            document.getElementById('totalInventoryItems').textContent = totalItems;
            document.getElementById('lowStockItems').textContent = lowStockItems;
            
            // Update stock alerts
            const alertsContainer = document.getElementById('stockAlerts');
            alertsContainer.innerHTML = '';
            
            const lowStockList = inventory.filter(item => item.quantity <= item.minStock);
            
            if (lowStockList.length === 0) {
                alertsContainer.innerHTML = '<p class="text-sm text-gray-500">Nenhum alerta de estoque</p>';
            } else {
                lowStockList.forEach(item => {
                    const div = document.createElement('div');
                    div.className = 'bg-red-50 p-2 rounded text-sm';
                    div.innerHTML = `<span class="font-medium">${item.name}</span> - ${item.quantity} ${item.unit} restantes`;
                    alertsContainer.appendChild(div);
                });
            }
        }

        // Equipment management
        function addEquipment() {
            const name = document.getElementById('equipmentName').value;
            const type = document.getElementById('equipmentType').value;
            const year = parseInt(document.getElementById('equipmentYear').value);
            const hours = parseFloat(document.getElementById('equipmentHours').value);
            const nextMaintenance = parseFloat(document.getElementById('equipmentNextMaintenance').value);
            const status = document.getElementById('equipmentStatus').value;
            
            if (!name || !year) {
                alert('Por favor, preencha nome e ano');
                return;
            }
            
            const equipmentItem = {
                id: Date.now(),
                name: name,
                type: type,
                year: year,
                hours: hours || 0,
                nextMaintenance: nextMaintenance || 0,
                status: status,
                addedAt: new Date().toISOString()
            };
            
            equipment.push(equipmentItem);
            renderEquipment();
            updateEquipmentSummary();
            
            // Clear form
            document.getElementById('equipmentName').value = '';
            document.getElementById('equipmentYear').value = '';
            document.getElementById('equipmentHours').value = '';
            document.getElementById('equipmentNextMaintenance').value = '';
        }

        function renderEquipment() {
            const container = document.getElementById('equipmentList');
            container.innerHTML = '';
            
            if (equipment.length === 0) {
                container.innerHTML = '<p class="text-gray-500 text-sm">Nenhum equipamento cadastrado ainda</p>';
                return;
            }
            
            equipment.forEach(item => {
                const div = document.createElement('div');
                const needsMaintenance = item.hours >= item.nextMaintenance && item.nextMaintenance > 0;
                const statusColor = {
                    'operacional': 'text-green-600 bg-green-50',
                    'manutencao': 'text-yellow-600 bg-yellow-50',
                    'quebrado': 'text-red-600 bg-red-50',
                    'inativo': 'text-gray-600 bg-gray-50'
                };
                
                div.className = `bg-white p-4 rounded-lg border ${needsMaintenance ? 'border-orange-200 bg-orange-50' : 'border-gray-200'}`;
                div.innerHTML = `
                    <div class="flex justify-between items-start">
                        <div class="flex-1">
                            <h4 class="font-medium">${item.name}</h4>
                            <p class="text-sm text-gray-600">${item.type} | ${item.year}</p>
                            <div class="flex items-center space-x-4 mt-2">
                                <span class="text-sm">⏱️ ${item.hours}h trabalhadas</span>
                                <span class="px-2 py-1 text-xs rounded-full ${statusColor[item.status]}">${item.status}</span>
                                ${needsMaintenance ? '<span class="text-xs bg-orange-100 text-orange-800 px-2 py-1 rounded-full">Manutenção necessária</span>' : ''}
                            </div>
                        </div>
                        <div class="flex space-x-2">
                            <button onclick="updateEquipmentHours(${item.id})" class="text-blue-600 hover:text-blue-800">
                                <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                                    <path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-2 15l-5-5 1.41-1.41L10 14.17l7.59-7.59L19 8l-9 9z"/>
                                </svg>
                            </button>
                            <button onclick="removeEquipment(${item.id})" class="text-red-600 hover:text-red-800">
                                <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                                    <path d="M19 6.41L17.59 5 12 10.59 6.41 5 5 6.41 10.59 12 5 17.59 6.41 19 12 13.41 17.59 19 19 17.59 13.41 12z"/>
                                </svg>
                            </button>
                        </div>
                    </div>
                `;
                container.appendChild(div);
            });
        }

        function updateEquipmentHours(id) {
            const item = equipment.find(e => e.id === id);
            if (item) {
                const newHours = parseFloat(prompt('Atualizar horas trabalhadas:', item.hours));
                if (newHours >= 0) {
                    item.hours = newHours;
                    renderEquipment();
                    updateEquipmentSummary();
                }
            }
        }

        function removeEquipment(id) {
            equipment = equipment.filter(item => item.id !== id);
            renderEquipment();
            updateEquipmentSummary();
        }

        function updateEquipmentSummary() {
            const operational = equipment.filter(item => item.status === 'operacional').length;
            const needsMaintenance = equipment.filter(item => 
                (item.hours >= item.nextMaintenance && item.nextMaintenance > 0) || 
                item.status === 'manutencao' || 
                item.status === 'quebrado'
            ).length;
            
            document.getElementById('operationalEquipment').textContent = operational;
            document.getElementById('maintenanceNeeded').textContent = needsMaintenance;
            
            // Update maintenance alerts
            const alertsContainer = document.getElementById('maintenanceAlerts');
            alertsContainer.innerHTML = '';
            
            const maintenanceList = equipment.filter(item => 
                item.hours >= item.nextMaintenance && item.nextMaintenance > 0
            );
            
            if (maintenanceList.length === 0) {
                alertsContainer.innerHTML = '<p class="text-sm text-gray-500">Nenhum alerta de manutenção</p>';
            } else {
                maintenanceList.forEach(item => {
                    const div = document.createElement('div');
                    div.className = 'bg-orange-50 p-2 rounded text-sm';
                    div.innerHTML = `<span class="font-medium">${item.name}</span> - ${item.hours}h (manutenção em ${item.nextMaintenance}h)`;
                    alertsContainer.appendChild(div);
                });
            }
        }

        // Weather functions
        function generateWeatherForecast() {
            const days = ['Dom', 'Seg', 'Ter', 'Qua', 'Qui', 'Sex', 'Sáb'];
            const container = document.getElementById('weeklyForecast');
            container.innerHTML = '';
            
            for (let i = 0; i < 7; i++) {
                const date = new Date();
                date.setDate(date.getDate() + i);
                const dayName = days[date.getDay()];
                const temp = Math.floor(Math.random() * 10) + 20; // 20-30°C
                const rain = Math.floor(Math.random() * 100);
                
                const div = document.createElement('div');
                div.className = 'bg-blue-50 p-4 rounded-lg text-center';
                div.innerHTML = `
                    <p class="font-medium text-sm">${dayName}</p>
                    <p class="text-xs text-gray-600">${date.getDate()}/${date.getMonth() + 1}</p>
                    <div class="text-2xl my-2">${rain > 70 ? '🌧️' : rain > 40 ? '⛅' : '☀️'}</div>
                    <p class="font-bold">${temp}°C</p>
                    <p class="text-xs text-gray-600">${rain}% chuva</p>
                `;
                container.appendChild(div);
            }
        }

        // Harvest functions
        function addHarvestRecord() {
            const date = document.getElementById('harvestDate').value;
            const sector = document.getElementById('harvestSector').value;
            const area = parseFloat(document.getElementById('harvestArea').value);
            const quantity = parseFloat(document.getElementById('harvestQuantity').value);
            const quality = document.getElementById('harvestQuality').value;
            const price = parseFloat(document.getElementById('harvestPrice').value);
            const notes = document.getElementById('harvestNotes').value;
            
            if (!date || !sector || !area || !quantity || !price) {
                alert('Por favor, preencha todos os campos obrigatórios');
                return;
            }
            
            const record = {
                id: Date.now(),
                date: new Date(date).toLocaleDateString('pt-BR'),
                sector: sector,
                area: area,
                quantity: quantity,
                quality: quality,
                price: price,
                notes: notes,
                revenue: quantity * price
            };
            
            harvestRecords.push(record);
            renderHarvestRecords();
            updateHarvestSummary();
            
            // Clear form
            document.getElementById('harvestSector').value = '';
            document.getElementById('harvestArea').value = '';
            document.getElementById('harvestQuantity').value = '';
            document.getElementById('harvestPrice').value = '';
            document.getElementById('harvestNotes').value = '';
        }

        function renderHarvestRecords() {
            const container = document.getElementById('harvestRecords');
            container.innerHTML = '';
            
            if (harvestRecords.length === 0) {
                container.innerHTML = '<p class="text-gray-500 text-sm">Nenhuma colheita registrada ainda</p>';
                return;
            }
            
            harvestRecords.forEach(record => {
                const div = document.createElement('div');
                div.className = 'bg-green-50 p-4 rounded-lg';
                div.innerHTML = `
                    <div class="flex justify-between items-start">
                        <div>
                            <h4 class="font-medium">${record.sector} - ${record.date}</h4>
                            <p class="text-sm text-gray-600">${record.area} alqueires | ${record.quantity} sacas | ${record.quality}</p>
                            <p class="text-sm font-semibold text-green-600">R$ ${record.revenue.toLocaleString('pt-BR', {minimumFractionDigits: 2})}</p>
                            ${record.notes ? `<p class="text-sm text-gray-500 mt-1">${record.notes}</p>` : ''}
                        </div>
                        <button onclick="removeHarvestRecord(${record.id})" class="text-red-600 hover:text-red-800">
                            <svg class="w-4 h-4" fill="currentColor" viewBox="0 0 24 24">
                                <path d="M19 6.41L17.59 5 12 10.59 6.41 5 5 6.41 10.59 12 5 17.59 6.41 19 12 13.41 17.59 19 19 17.59 13.41 12z"/>
                            </svg>
                        </button>
                    </div>
                `;
                container.appendChild(div);
            });
        }

        function removeHarvestRecord(id) {
            harvestRecords = harvestRecords.filter(record => record.id !== id);
            renderHarvestRecords();
            updateHarvestSummary();
        }

        function updateHarvestSummary() {
            const totalHarvested = harvestRecords.reduce((sum, r) => sum + r.quantity, 0);
            const totalArea = harvestRecords.reduce((sum, r) => sum + r.area, 0);
            const totalRevenue = harvestRecords.reduce((sum, r) => sum + r.revenue, 0);
            const averageProductivity = totalArea > 0 ? totalHarvested / totalArea : 0;
            const averagePrice = totalHarvested > 0 ? totalRevenue / totalHarvested : 0;
            
            document.getElementById('totalHarvested').textContent = `${totalHarvested} sacas`;
            document.getElementById('averageProductivity').textContent = `${averageProductivity.toFixed(1)} sc/alq`;
            document.getElementById('totalHarvestRevenue').textContent = `R$ ${totalRevenue.toLocaleString('pt-BR')}`;
            document.getElementById('averagePrice').textContent = `R$ ${averagePrice.toFixed(2)}/sc`;
        }

        function calculateHarvestProjection() {
            const totalArea = parseFloat(document.getElementById('totalArea').textContent) || 0;
            if (totalArea === 0) {
                alert('Primeiro cadastre a área total da propriedade');
                return;
            }
            
            const averageProductivity = harvestRecords.length > 0 ? 
                harvestRecords.reduce((sum, r) => sum + (r.quantity / r.area), 0) / harvestRecords.length : 30;
            
            const projectedHarvest = totalArea * averageProductivity;
            const estimatedPrice = 450; // Preço estimado por saca
            const projectedRevenue = projectedHarvest * estimatedPrice;
            
            alert(`Projeção da Safra:\n\nProdução estimada: ${projectedHarvest.toFixed(0)} sacas\nReceita estimada: R$ ${projectedRevenue.toLocaleString('pt-BR')}\nProdutividade média: ${averageProductivity.toFixed(1)} sc/alq`);
        }

        // Report functions
        function generateReport() {
            const reportType = document.getElementById('reportType').value;
            const startDate = document.getElementById('reportStartDate').value;
            const endDate = document.getElementById('reportEndDate').value;
            const container = document.getElementById('reportDisplay');
            
            if (!startDate || !endDate) {
                alert('Por favor, selecione as datas do relatório');
                return;
            }
            
            let reportContent = '';
            
            switch (reportType) {
                case 'financial':
                    reportContent = generateFinancialReport(startDate, endDate);
                    break;
                case 'production':
                    reportContent = generateProductionReport(startDate, endDate);
                    break;
                case 'inventory':
                    reportContent = generateInventoryReport();
                    break;
                case 'tasks':
                    reportContent = generateTasksReport(startDate, endDate);
                    break;
                case 'equipment':
                    reportContent = generateEquipmentReport();
                    break;
                default:
                    reportContent = '<p class="text-gray-500">Tipo de relatório não encontrado</p>';
            }
            
            container.innerHTML = reportContent;
        }

        function generateFinancialReport(startDate, endDate) {
            const filteredRevenues = revenues.filter(r => {
                const recordDate = new Date(r.date.split('/').reverse().join('-'));
                return recordDate >= new Date(startDate) && recordDate <= new Date(endDate);
            });
            
            const filteredExpenses = expenses.filter(e => {
                const recordDate = new Date(e.date.split('/').reverse().join('-'));
                return recordDate >= new Date(startDate) && recordDate <= new Date(endDate);
            });
            
            const totalRevenue = filteredRevenues.reduce((sum, r) => sum + r.amount, 0);
            const totalExpenses = filteredExpenses.reduce((sum, e) => sum + e.amount, 0);
            const netProfit = totalRevenue - totalExpenses;
            
            return `
                <div class="space-y-4">
                    <h4 class="text-lg font-semibold">Relatório Financeiro</h4>
                    <div class="grid grid-cols-3 gap-4">
                        <div class="bg-green-50 p-4 rounded-lg">
                            <p class="text-sm text-gray-600">Receitas</p>
                            <p class="text-xl font-bold text-green-600">R$ ${totalRevenue.toLocaleString('pt-BR', {minimumFractionDigits: 2})}</p>
                        </div>
                        <div class="bg-red-50 p-4 rounded-lg">
                            <p class="text-sm text-gray-600">Despesas</p>
                            <p class="text-xl font-bold text-red-600">R$ ${totalExpenses.toLocaleString('pt-BR', {minimumFractionDigits: 2})}</p>
                        </div>
                        <div class="bg-blue-50 p-4 rounded-lg">
                            <p class="text-sm text-gray-600">Lucro Líquido</p>
                            <p class="text-xl font-bold text-blue-600">R$ ${netProfit.toLocaleString('pt-BR', {minimumFractionDigits: 2})}</p>
                        </div>
                    </div>
                    <p class="text-sm text-gray-600">Período: ${new Date(startDate).toLocaleDateString('pt-BR')} a ${new Date(endDate).toLocaleDateString('pt-BR')}</p>
                </div>
            `;
        }

        function generateProductionReport(startDate, endDate) {
            const filteredHarvests = harvestRecords.filter(h => {
                const recordDate = new Date(h.date.split('/').reverse().join('-'));
                return recordDate >= new Date(startDate) && recordDate <= new Date(endDate);
            });
            
            const totalProduction = filteredHarvests.reduce((sum, h) => sum + h.quantity, 0);
            const totalArea = filteredHarvests.reduce((sum, h) => sum + h.area, 0);
            const averageProductivity = totalArea > 0 ? totalProduction / totalArea : 0;
            
            return `
                <div class="space-y-4">
                    <h4 class="text-lg font-semibold">Relatório de Produção</h4>
                    <div class="grid grid-cols-3 gap-4">
                        <div class="bg-green-50 p-4 rounded-lg">
                            <p class="text-sm text-gray-600">Produção Total</p>
                            <p class="text-xl font-bold text-green-600">${totalProduction} sacas</p>
                        </div>
                        <div class="bg-blue-50 p-4 rounded-lg">
                            <p class="text-sm text-gray-600">Área Colhida</p>
                            <p class="text-xl font-bold text-blue-600">${totalArea} alqueires</p>
                        </div>
                        <div class="bg-yellow-50 p-4 rounded-lg">
                            <p class="text-sm text-gray-600">Produtividade</p>
                            <p class="text-xl font-bold text-yellow-600">${averageProductivity.toFixed(1)} sc/alq</p>
                        </div>
                    </div>
                    <p class="text-sm text-gray-600">Período: ${new Date(startDate).toLocaleDateString('pt-BR')} a ${new Date(endDate).toLocaleDateString('pt-BR')}</p>
                </div>
            `;
        }

        function generateInventoryReport() {
            const totalItems = inventory.length;
            const lowStockItems = inventory.filter(item => item.quantity <= item.minStock).length;
            const totalValue = inventory.reduce((sum, item) => sum + (item.quantity * item.price), 0);
            
            return `
                <div class="space-y-4">
                    <h4 class="text-lg font-semibold">Relatório de Estoque</h4>
                    <div class="grid grid-cols-3 gap-4">
                        <div class="bg-blue-50 p-4 rounded-lg">
                            <p class="text-sm text-gray-600">Total de Itens</p>
                            <p class="text-xl font-bold text-blue-600">${totalItems}</p>
                        </div>
                        <div class="bg-red-50 p-4 rounded-lg">
                            <p class="text-sm text-gray-600">Estoque Baixo</p>
                            <p class="text-xl font-bold text-red-600">${lowStockItems}</p>
                        </div>
                        <div class="bg-green-50 p-4 rounded-lg">
                            <p class="text-sm text-gray-600">Valor Total</p>
                            <p class="text-xl font-bold text-green-600">R$ ${totalValue.toLocaleString('pt-BR', {minimumFractionDigits: 2})}</p>
                        </div>
                    </div>
                </div>
            `;
        }

        function generateTasksReport(startDate, endDate) {
            const filteredTasks = tasks.filter(t => {
                const taskDate = new Date(t.date);
                return taskDate >= new Date(startDate) && taskDate <= new Date(endDate);
            });
            
            const completedTasks = filteredTasks.filter(t => t.completed).length;
            const pendingTasks = filteredTasks.filter(t => !t.completed).length;
            const overdueTasks = filteredTasks.filter(t => !t.completed && new Date(t.date) < new Date()).length;
            
            return `
                <div class="space-y-4">
                    <h4 class="text-lg font-semibold">Relatório de Tarefas</h4>
                    <div class="grid grid-cols-3 gap-4">
                        <div class="bg-green-50 p-4 rounded-lg">
                            <p class="text-sm text-gray-600">Concluídas</p>
                            <p class="text-xl font-bold text-green-600">${completedTasks}</p>
                        </div>
                        <div class="bg-yellow-50 p-4 rounded-lg">
                            <p class="text-sm text-gray-600">Pendentes</p>
                            <p class="text-xl font-bold text-yellow-600">${pendingTasks}</p>
                        </div>
                        <div class="bg-red-50 p-4 rounded-lg">
                            <p class="text-sm text-gray-600">Atrasadas</p>
                            <p class="text-xl font-bold text-red-600">${overdueTasks}</p>
                        </div>
                    </div>
                    <p class="text-sm text-gray-600">Período: ${new Date(startDate).toLocaleDateString('pt-BR')} a ${new Date(endDate).toLocaleDateString('pt-BR')}</p>
                </div>
            `;
        }

        function generateEquipmentReport() {
            const totalEquipment = equipment.length;
            const operational = equipment.filter(e => e.status === 'operacional').length;
            const needsMaintenance = equipment.filter(e => e.status === 'manutencao' || e.status === 'quebrado').length;
            
            return `
                <div class="space-y-4">
                    <h4 class="text-lg font-semibold">Relatório de Equipamentos</h4>
                    <div class="grid grid-cols-3 gap-4">
                        <div class="bg-blue-50 p-4 rounded-lg">
                            <p class="text-sm text-gray-600">Total</p>
                            <p class="text-xl font-bold text-blue-600">${totalEquipment}</p>
                        </div>
                        <div class="bg-green-50 p-4 rounded-lg">
                            <p class="text-sm text-gray-600">Operacionais</p>
                            <p class="text-xl font-bold text-green-600">${operational}</p>
                        </div>
                        <div class="bg-red-50 p-4 rounded-lg">
                            <p class="text-sm text-gray-600">Manutenção</p>
                            <p class="text-xl font-bold text-red-600">${needsMaintenance}</p>
                        </div>
                    </div>
                </div>
            `;
        }

        // Calculator functions
        function convertUnits() {
            const hectares = parseFloat(document.getElementById('hectares').value) || 0;
            const alqueires = hectares * 0.4132; // 1 hectare = 0.4132 alqueires paulistas
            const squareMeters = hectares * 10000;
            
            document.getElementById('alqueires').value = alqueires.toFixed(4);
            document.getElementById('squareMeters').value = squareMeters.toFixed(0);
        }

        function convertFromAlqueires() {
            const alqueires = parseFloat(document.getElementById('alqueires').value) || 0;
            const hectares = alqueires / 0.4132;
            const squareMeters = alqueires * 24200;
            
            document.getElementById('hectares').value = hectares.toFixed(4);
            document.getElementById('squareMeters').value = squareMeters.toFixed(0);
        }

        function calculateProductivity() {
            const production = parseFloat(document.getElementById('production').value);
            const area = parseFloat(document.getElementById('productivityArea').value);
            
            if (!production || !area) {
                alert('Por favor, preencha produção e área');
                return;
            }
            
            const productivity = production / area;
            document.getElementById('productivityValue').textContent = `${productivity.toFixed(2)} sacas por alqueire`;
            document.getElementById('productivityResult').classList.remove('hidden');
        }

        function calculateCostPerBag() {
            const totalCost = parseFloat(document.getElementById('totalCost').value);
            const totalProduction = parseFloat(document.getElementById('totalProduction').value);
            
            if (!totalCost || !totalProduction) {
                alert('Por favor, preencha custo total e produção');
                return;
            }
            
            const costPerBag = totalCost / totalProduction;
            document.getElementById('costPerBagValue').textContent = `R$ ${costPerBag.toFixed(2)} por saca`;
            document.getElementById('costPerBagResult').classList.remove('hidden');
        }

        // Dashboard update function
        function updateDashboard() {
            // Update pending tasks
            const pendingTasksToday = tasks.filter(task => 
                !task.completed && 
                new Date(task.date).toDateString() === new Date().toDateString()
            ).length;
            document.getElementById('pendingTasks').textContent = pendingTasksToday;
            
            // Update upcoming tasks
            const upcomingTasks = tasks.filter(task => 
                !task.completed && 
                new Date(task.date) >= new Date()
            ).slice(0, 5);
            
            const upcomingContainer = document.getElementById('upcomingTasks');
            upcomingContainer.innerHTML = '';
            
            if (upcomingTasks.length === 0) {
                upcomingContainer.innerHTML = '<p class="text-gray-500 text-sm">Nenhuma tarefa pendente</p>';
            } else {
                upcomingTasks.forEach(task => {
                    const div = document.createElement('div');
                    div.className = `task-priority-${task.priority} bg-white p-2 rounded text-sm`;
                    div.innerHTML = `
                        <p class="font-medium">${task.title}</p>
                        <p class="text-xs text-gray-600">${new Date(task.date).toLocaleDateString('pt-BR')} | ${task.category}</p>
                    `;
                    upcomingContainer.appendChild(div);
                });
            }
            
            // Update quick stats
            const monthlyProfit = revenues.reduce((sum, r) => sum + r.amount, 0) - expenses.reduce((sum, e) => sum + e.amount, 0);
            const completedTasksCount = tasks.filter(t => t.completed).length;
            const activeEquipmentCount = equipment.filter(e => e.status === 'operacional').length;
            const lowStockCount = inventory.filter(item => item.quantity <= item.minStock).length;
            
            document.getElementById('monthlyProfit').textContent = `R$ ${monthlyProfit.toLocaleString('pt-BR')}`;
            document.getElementById('completedTasksCount').textContent = completedTasksCount;
            document.getElementById('activeEquipmentCount').textContent = activeEquipmentCount;
            document.getElementById('lowStockCount').textContent = lowStockCount;
        }

        // Employee management functions
        function addEmployee() {
            const name = document.getElementById('employeeName').value;
            const role = document.getElementById('employeeRole').value;
            const salary = parseFloat(document.getElementById('employeeSalary').value);
            const hireDate = document.getElementById('employeeHireDate').value;
            const cpf = document.getElementById('employeeCPF').value;
            const rg = document.getElementById('employeeRG').value;
            const phone = document.getElementById('employeePhone').value;
            const email = document.getElementById('employeeEmail').value;
            const address = document.getElementById('employeeAddress').value;
            const birthDate = document.getElementById('employeeBirthDate').value;
            const maritalStatus = document.getElementById('employeeMaritalStatus').value;
            const education = document.getElementById('employeeEducation').value;
            const bank = document.getElementById('employeeBank').value;
            const bankAccount = document.getElementById('employeeBankAccount').value;
            const emergencyContact = document.getElementById('employeeEmergencyContact').value;
            const emergencyPhone = document.getElementById('employeeEmergencyPhone').value;
            const status = document.getElementById('employeeStatus').value;
            const contractType = document.getElementById('employeeContractType').value;
            const notes = document.getElementById('employeeNotes').value;
            
            if (!name || isNaN(salary) || !hireDate) {
                alert('Por favor, preencha nome, salário (pode ser 0 para pagamento por produção) e data de admissão');
                return;
            }
            
            if (salary < 0) {
                alert('O salário não pode ser negativo');
                return;
            }
            
            const employee = {
                id: Date.now(),
                name: name,
                role: role,
                salary: salary,
                hireDate: new Date(hireDate).toLocaleDateString('pt-BR'),
                cpf: cpf,
                rg: rg,
                phone: phone,
                email: email,
                address: address,
                birthDate: birthDate ? new Date(birthDate).toLocaleDateString('pt-BR') : '',
                maritalStatus: maritalStatus,
                education: education,
                bank: bank,
                bankAccount: bankAccount,
                emergencyContact: emergencyContact,
                emergencyPhone: emergencyPhone,
                status: status,
                contractType: contractType,
                notes: notes,
                addedAt: new Date().toISOString()
            };
            
            employees.push(employee);
            renderEmployees();
            updateEmployeeSummary();
            updatePayrollEmployeeSelect();
            updateProductionEmployeeSelects();
            
            // Clear form
            clearEmployeeForm();
            
            alert(`Funcionário ${name} cadastrado com sucesso!`);
        }

        function clearEmployeeForm() {
            document.getElementById('employeeName').value = '';
            document.getElementById('employeeSalary').value = '';
            document.getElementById('employeeHireDate').value = '';
            document.getElementById('employeeCPF').value = '';
            document.getElementById('employeeRG').value = '';
            document.getElementById('employeePhone').value = '';
            document.getElementById('employeeEmail').value = '';
            document.getElementById('employeeAddress').value = '';
            document.getElementById('employeeBirthDate').value = '';
            document.getElementById('employeeMaritalStatus').value = '';
            document.getElementById('employeeEducation').value = '';
            document.getElementById('employeeBank').value = '';
            document.getElementById('employeeBankAccount').value = '';
            document.getElementById('employeeEmergencyContact').value = '';
            document.getElementById('employeeEmergencyPhone').value = '';
            document.getElementById('employeeNotes').value = '';
        }

        function renderEmployees() {
            const container = document.getElementById('employeeList');
            container.innerHTML = '';
            
            const filteredEmployees = filterEmployeesArray();
            
            if (filteredEmployees.length === 0) {
                container.innerHTML = '<p class="text-gray-500 text-sm">Nenhum funcionário encontrado</p>';
                return;
            }
            
            filteredEmployees.forEach(employee => {
                const div = document.createElement('div');
                const statusColor = {
                    'ativo': 'text-green-600 bg-green-50',
                    'ferias': 'text-blue-600 bg-blue-50',
                    'afastado': 'text-yellow-600 bg-yellow-50',
                    'licenca': 'text-purple-600 bg-purple-50',
                    'demitido': 'text-red-600 bg-red-50'
                };
                
                div.className = 'bg-white p-4 rounded-lg border border-gray-200';
                div.innerHTML = `
                    <div class="flex justify-between items-start">
                        <div class="flex-1">
                            <div class="flex items-center space-x-2 mb-1">
                                <h4 class="font-medium">${employee.name}</h4>
                                <span class="px-2 py-1 text-xs rounded-full ${statusColor[employee.status]}">${employee.status}</span>
                                ${employee.contractType ? `<span class="px-2 py-1 text-xs rounded-full bg-gray-100 text-gray-700">${employee.contractType}</span>` : ''}
                            </div>
                            <p class="text-sm text-gray-600">${employee.role} | Admissão: ${employee.hireDate}</p>
                            <div class="flex items-center space-x-4 mt-2">
                                <span class="text-sm font-semibold ${employee.salary > 0 ? 'text-green-600' : 'text-blue-600'}">${employee.salary > 0 ? `R$ ${employee.salary.toLocaleString('pt-BR', {minimumFractionDigits: 2})}` : 'Pagamento por Produção'}</span>
                                ${employee.phone ? `<span class="text-sm text-gray-500">📞 ${employee.phone}</span>` : ''}
                                ${employee.email ? `<span class="text-sm text-gray-500">📧 ${employee.email}</span>` : ''}
                            </div>
                            ${employee.cpf ? `<p class="text-xs text-gray-500 mt-1">CPF: ${employee.cpf}</p>` : ''}
                            ${employee.emergencyContact ? `<p class="text-xs text-gray-500">Emergência: ${employee.emergencyContact} ${employee.emergencyPhone ? `- ${employee.emergencyPhone}` : ''}</p>` : ''}
                            ${employee.notes ? `<p class="text-sm text-gray-500 mt-1 italic">${employee.notes}</p>` : ''}
                        </div>
                        <div class="flex space-x-2">
                            <button onclick="viewEmployeeDetails(${employee.id})" class="text-green-600 hover:text-green-800" title="Ver detalhes">
                                <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                                    <path d="M12 4.5C7 4.5 2.73 7.61 1 12c1.73 4.39 6 7.5 11 7.5s9.27-3.11 11-7.5c-1.73-4.39-6-7.5-11-7.5zM12 17c-2.76 0-5-2.24-5-5s2.24-5 5-5 5 2.24 5 5-2.24 5-5 5zm0-8c-1.66 0-3 1.34-3 3s1.34 3 3 3 3-1.34 3-3-1.34-3-3-3z"/>
                                </svg>
                            </button>
                            <button onclick="editEmployee(${employee.id})" class="text-blue-600 hover:text-blue-800" title="Editar">
                                <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                                    <path d="M3 17.25V21h3.75L17.81 9.94l-3.75-3.75L3 17.25zM20.71 7.04c.39-.39.39-1.02 0-1.41l-2.34-2.34c-.39-.39-1.02-.39-1.41 0l-1.83 1.83 3.75 3.75 1.83-1.83z"/>
                                </svg>
                            </button>
                            ${employee.status === 'ativo' ? `
                            <button onclick="dismissEmployee(${employee.id})" class="text-orange-600 hover:text-orange-800" title="Demitir">
                                <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                                    <path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm5 11H7v-2h10v2z"/>
                                </svg>
                            </button>
                            ` : ''}
                            <button onclick="confirmDeleteEmployee(${employee.id})" class="text-red-600 hover:text-red-800" title="Excluir permanentemente">
                                <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                                    <path d="M6 19c0 1.1.9 2 2 2h8c1.1 0 2-.9 2-2V7H6v12zM19 4h-3.5l-1-1h-5l-1 1H5v2h14V4z"/>
                                </svg>
                            </button>
                        </div>
                    </div>
                `;
                container.appendChild(div);
            });
        }

        function filterEmployeesArray() {
            const statusFilter = document.getElementById('employeeFilterStatus').value;
            
            return employees.filter(employee => {
                return statusFilter === 'all' || employee.status === statusFilter;
            });
        }

        function filterEmployees() {
            renderEmployees();
        }

        function editEmployee(id) {
            const employee = employees.find(e => e.id === id);
            if (!employee) return;
            
            // Create modal for editing
            const modal = document.createElement('div');
            modal.className = 'fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center z-50 p-4';
            modal.innerHTML = `
                <div class="bg-white rounded-xl shadow-lg max-w-4xl w-full max-h-[90vh] overflow-y-auto">
                    <div class="p-6">
                        <div class="flex justify-between items-center mb-6">
                            <h3 class="text-xl font-semibold">Editar Funcionário: ${employee.name}</h3>
                            <button onclick="closeEditModal()" class="text-gray-500 hover:text-gray-700">
                                <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24">
                                    <path d="M19 6.41L17.59 5 12 10.59 6.41 5 5 6.41 10.59 12 5 17.59 6.41 19 12 13.41 17.59 19 19 17.59 13.41 12z"/>
                                </svg>
                            </button>
                        </div>
                        
                        <form id="editEmployeeForm" class="space-y-4">
                            <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                                <div>
                                    <label class="block text-sm font-medium text-gray-700 mb-2">Nome completo</label>
                                    <input type="text" id="editEmployeeName" value="${employee.name}" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                                </div>
                                <div>
                                    <label class="block text-sm font-medium text-gray-700 mb-2">Função</label>
                                    <select id="editEmployeeRole" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                                        <option value="operador-campo" ${employee.role === 'operador-campo' ? 'selected' : ''}>Operador de Campo</option>
                                        <option value="tratorista" ${employee.role === 'tratorista' ? 'selected' : ''}>Tratorista</option>
                                        <option value="aplicador" ${employee.role === 'aplicador' ? 'selected' : ''}>Aplicador de Defensivos</option>
                                        <option value="colhedor" ${employee.role === 'colhedor' ? 'selected' : ''}>Colhedor</option>
                                        <option value="colhedor-selecionador" ${employee.role === 'colhedor-selecionador' ? 'selected' : ''}>Colhedor Selecionador</option>
                                        <option value="irrigador" ${employee.role === 'irrigador' ? 'selected' : ''}>Irrigador</option>
                                        <option value="podador" ${employee.role === 'podador' ? 'selected' : ''}>Podador</option>
                                        <option value="mecanico" ${employee.role === 'mecanico' ? 'selected' : ''}>Mecânico</option>
                                        <option value="eletricista" ${employee.role === 'eletricista' ? 'selected' : ''}>Eletricista</option>
                                        <option value="soldador" ${employee.role === 'soldador' ? 'selected' : ''}>Soldador</option>
                                        <option value="motorista" ${employee.role === 'motorista' ? 'selected' : ''}>Motorista</option>
                                        <option value="operador-maquinas" ${employee.role === 'operador-maquinas' ? 'selected' : ''}>Operador de Máquinas</option>
                                        <option value="supervisor" ${employee.role === 'supervisor' ? 'selected' : ''}>Supervisor de Campo</option>
                                        <option value="encarregado" ${employee.role === 'encarregado' ? 'selected' : ''}>Encarregado</option>
                                        <option value="tecnico-agricola" ${employee.role === 'tecnico-agricola' ? 'selected' : ''}>Técnico Agrícola</option>
                                        <option value="engenheiro" ${employee.role === 'engenheiro' ? 'selected' : ''}>Engenheiro Agrônomo</option>
                                        <option value="veterinario" ${employee.role === 'veterinario' ? 'selected' : ''}>Veterinário</option>
                                        <option value="administrativo" ${employee.role === 'administrativo' ? 'selected' : ''}>Administrativo</option>
                                        <option value="contador" ${employee.role === 'contador' ? 'selected' : ''}>Contador</option>
                                        <option value="recursos-humanos" ${employee.role === 'recursos-humanos' ? 'selected' : ''}>Recursos Humanos</option>
                                        <option value="gerente" ${employee.role === 'gerente' ? 'selected' : ''}>Gerente</option>
                                        <option value="coordenador" ${employee.role === 'coordenador' ? 'selected' : ''}>Coordenador</option>
                                        <option value="diretor" ${employee.role === 'diretor' ? 'selected' : ''}>Diretor</option>
                                        <option value="vigilante" ${employee.role === 'vigilante' ? 'selected' : ''}>Vigilante</option>
                                        <option value="porteiro" ${employee.role === 'porteiro' ? 'selected' : ''}>Porteiro</option>
                                        <option value="cozinheiro" ${employee.role === 'cozinheiro' ? 'selected' : ''}>Cozinheiro</option>
                                        <option value="auxiliar-limpeza" ${employee.role === 'auxiliar-limpeza' ? 'selected' : ''}>Auxiliar de Limpeza</option>
                                        <option value="jardineiro" ${employee.role === 'jardineiro' ? 'selected' : ''}>Jardineiro</option>
                                        <option value="caseiro" ${employee.role === 'caseiro' ? 'selected' : ''}>Caseiro</option>
                                        <option value="outros" ${employee.role === 'outros' ? 'selected' : ''}>Outros</option>
                                    </select>
                                </div>
                            </div>
                            
                            <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                                <div>
                                    <label class="block text-sm font-medium text-gray-700 mb-2">Salário (R$)</label>
                                    <input type="number" id="editEmployeeSalary" value="${employee.salary}" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" min="0">
                                </div>
                                <div>
                                    <label class="block text-sm font-medium text-gray-700 mb-2">Status</label>
                                    <select id="editEmployeeStatus" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                                        <option value="ativo" ${employee.status === 'ativo' ? 'selected' : ''}>Ativo</option>
                                        <option value="ferias" ${employee.status === 'ferias' ? 'selected' : ''}>Férias</option>
                                        <option value="afastado" ${employee.status === 'afastado' ? 'selected' : ''}>Afastado</option>
                                        <option value="licenca" ${employee.status === 'licenca' ? 'selected' : ''}>Licença</option>
                                        <option value="demitido" ${employee.status === 'demitido' ? 'selected' : ''}>Demitido</option>
                                    </select>
                                </div>
                            </div>
                            
                            <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                                <div>
                                    <label class="block text-sm font-medium text-gray-700 mb-2">CPF</label>
                                    <input type="text" id="editEmployeeCPF" value="${employee.cpf || ''}" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                                </div>
                                <div>
                                    <label class="block text-sm font-medium text-gray-700 mb-2">RG</label>
                                    <input type="text" id="editEmployeeRG" value="${employee.rg || ''}" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                                </div>
                            </div>
                            
                            <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                                <div>
                                    <label class="block text-sm font-medium text-gray-700 mb-2">Telefone</label>
                                    <input type="tel" id="editEmployeePhone" value="${employee.phone || ''}" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                                </div>
                                <div>
                                    <label class="block text-sm font-medium text-gray-700 mb-2">Email</label>
                                    <input type="email" id="editEmployeeEmail" value="${employee.email || ''}" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                                </div>
                            </div>
                            
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Endereço</label>
                                <input type="text" id="editEmployeeAddress" value="${employee.address || ''}" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                            </div>
                            
                            <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
                                <div>
                                    <label class="block text-sm font-medium text-gray-700 mb-2">Data de Nascimento</label>
                                    <input type="date" id="editEmployeeBirthDate" value="${employee.birthDate ? employee.birthDate.split('/').reverse().join('-') : ''}" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                                </div>
                                <div>
                                    <label class="block text-sm font-medium text-gray-700 mb-2">Estado Civil</label>
                                    <select id="editEmployeeMaritalStatus" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                                        <option value="">Selecione</option>
                                        <option value="solteiro" ${employee.maritalStatus === 'solteiro' ? 'selected' : ''}>Solteiro(a)</option>
                                        <option value="casado" ${employee.maritalStatus === 'casado' ? 'selected' : ''}>Casado(a)</option>
                                        <option value="divorciado" ${employee.maritalStatus === 'divorciado' ? 'selected' : ''}>Divorciado(a)</option>
                                        <option value="viuvo" ${employee.maritalStatus === 'viuvo' ? 'selected' : ''}>Viúvo(a)</option>
                                        <option value="uniao-estavel" ${employee.maritalStatus === 'uniao-estavel' ? 'selected' : ''}>União Estável</option>
                                    </select>
                                </div>
                                <div>
                                    <label class="block text-sm font-medium text-gray-700 mb-2">Escolaridade</label>
                                    <select id="editEmployeeEducation" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                                        <option value="">Selecione</option>
                                        <option value="fundamental-incompleto" ${employee.education === 'fundamental-incompleto' ? 'selected' : ''}>Fundamental Incompleto</option>
                                        <option value="fundamental-completo" ${employee.education === 'fundamental-completo' ? 'selected' : ''}>Fundamental Completo</option>
                                        <option value="medio-incompleto" ${employee.education === 'medio-incompleto' ? 'selected' : ''}>Médio Incompleto</option>
                                        <option value="medio-completo" ${employee.education === 'medio-completo' ? 'selected' : ''}>Médio Completo</option>
                                        <option value="tecnico" ${employee.education === 'tecnico' ? 'selected' : ''}>Técnico</option>
                                        <option value="superior-incompleto" ${employee.education === 'superior-incompleto' ? 'selected' : ''}>Superior Incompleto</option>
                                        <option value="superior-completo" ${employee.education === 'superior-completo' ? 'selected' : ''}>Superior Completo</option>
                                        <option value="pos-graduacao" ${employee.education === 'pos-graduacao' ? 'selected' : ''}>Pós-graduação</option>
                                    </select>
                                </div>
                            </div>
                            
                            <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                                <div>
                                    <label class="block text-sm font-medium text-gray-700 mb-2">Banco</label>
                                    <input type="text" id="editEmployeeBank" value="${employee.bank || ''}" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                                </div>
                                <div>
                                    <label class="block text-sm font-medium text-gray-700 mb-2">Agência e Conta</label>
                                    <input type="text" id="editEmployeeBankAccount" value="${employee.bankAccount || ''}" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                                </div>
                            </div>
                            
                            <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                                <div>
                                    <label class="block text-sm font-medium text-gray-700 mb-2">Contato de Emergência</label>
                                    <input type="text" id="editEmployeeEmergencyContact" value="${employee.emergencyContact || ''}" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                                </div>
                                <div>
                                    <label class="block text-sm font-medium text-gray-700 mb-2">Telefone de Emergência</label>
                                    <input type="tel" id="editEmployeeEmergencyPhone" value="${employee.emergencyPhone || ''}" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                                </div>
                            </div>
                            
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Tipo de Contrato</label>
                                <select id="editEmployeeContractType" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
                                    <option value="clt" ${employee.contractType === 'clt' ? 'selected' : ''}>CLT</option>
                                    <option value="temporario" ${employee.contractType === 'temporario' ? 'selected' : ''}>Temporário</option>
                                    <option value="terceirizado" ${employee.contractType === 'terceirizado' ? 'selected' : ''}>Terceirizado</option>
                                    <option value="cooperado" ${employee.contractType === 'cooperado' ? 'selected' : ''}>Cooperado</option>
                                    <option value="autonomo" ${employee.contractType === 'autonomo' ? 'selected' : ''}>Autônomo</option>
                                    <option value="estagiario" ${employee.contractType === 'estagiario' ? 'selected' : ''}>Estagiário</option>
                                </select>
                            </div>
                            
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-2">Observações</label>
                                <textarea id="editEmployeeNotes" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" rows="3">${employee.notes || ''}</textarea>
                            </div>
                            
                            <div class="flex justify-end space-x-3 pt-4 border-t">
                                <button type="button" onclick="closeEditModal()" class="px-4 py-2 text-gray-600 border border-gray-300 rounded-lg hover:bg-gray-50">
                                    Cancelar
                                </button>
                                <button type="button" onclick="saveEmployeeChanges(${id})" class="px-4 py-2 bg-blue-600 text-white rounded-lg hover:bg-blue-700">
                                    Salvar Alterações
                                </button>
                            </div>
                        </form>
                    </div>
                </div>
            `;
            
            document.body.appendChild(modal);
        }
        
        function closeEditModal() {
            const modal = document.querySelector('.fixed.inset-0');
            if (modal) {
                modal.remove();
            }
        }
        
        function saveEmployeeChanges(id) {
            const employee = employees.find(e => e.id === id);
            if (!employee) return;
            
            // Get all form values
            const name = document.getElementById('editEmployeeName').value;
            const role = document.getElementById('editEmployeeRole').value;
            const salary = parseFloat(document.getElementById('editEmployeeSalary').value);
            const status = document.getElementById('editEmployeeStatus').value;
            const cpf = document.getElementById('editEmployeeCPF').value;
            const rg = document.getElementById('editEmployeeRG').value;
            const phone = document.getElementById('editEmployeePhone').value;
            const email = document.getElementById('editEmployeeEmail').value;
            const address = document.getElementById('editEmployeeAddress').value;
            const birthDate = document.getElementById('editEmployeeBirthDate').value;
            const maritalStatus = document.getElementById('editEmployeeMaritalStatus').value;
            const education = document.getElementById('editEmployeeEducation').value;
            const bank = document.getElementById('editEmployeeBank').value;
            const bankAccount = document.getElementById('editEmployeeBankAccount').value;
            const emergencyContact = document.getElementById('editEmployeeEmergencyContact').value;
            const emergencyPhone = document.getElementById('editEmployeeEmergencyPhone').value;
            const contractType = document.getElementById('editEmployeeContractType').value;
            const notes = document.getElementById('editEmployeeNotes').value;
            
            if (!name || isNaN(salary) || salary < 0) {
                alert('Por favor, preencha o nome e um salário válido (pode ser 0 para pagamento por produção)');
                return;
            }
            
            // Update employee data
            employee.name = name;
            employee.role = role;
            employee.salary = salary;
            employee.status = status;
            employee.cpf = cpf;
            employee.rg = rg;
            employee.phone = phone;
            employee.email = email;
            employee.address = address;
            employee.birthDate = birthDate ? new Date(birthDate).toLocaleDateString('pt-BR') : '';
            employee.maritalStatus = maritalStatus;
            employee.education = education;
            employee.bank = bank;
            employee.bankAccount = bankAccount;
            employee.emergencyContact = emergencyContact;
            employee.emergencyPhone = emergencyPhone;
            employee.contractType = contractType;
            employee.notes = notes;
            
            // Close modal and refresh displays
            closeEditModal();
            renderEmployees();
            updateEmployeeSummary();
            updatePayrollEmployeeSelect();
            
            alert(`Dados de ${name} atualizados com sucesso!`);
        }

        function viewEmployeeDetails(id) {
            const employee = employees.find(e => e.id === id);
            if (employee) {
                let details = `
📋 DETALHES DO FUNCIONÁRIO

👤 DADOS PESSOAIS:
Nome: ${employee.name}
CPF: ${employee.cpf || 'Não informado'}
RG: ${employee.rg || 'Não informado'}
Data de Nascimento: ${employee.birthDate || 'Não informado'}
Estado Civil: ${employee.maritalStatus || 'Não informado'}
Escolaridade: ${employee.education || 'Não informado'}

📞 CONTATO:
Telefone: ${employee.phone || 'Não informado'}
Email: ${employee.email || 'Não informado'}
Endereço: ${employee.address || 'Não informado'}

🏢 DADOS PROFISSIONAIS:
Função: ${employee.role}
Salário: ${employee.salary > 0 ? `R$ ${employee.salary.toLocaleString('pt-BR', {minimumFractionDigits: 2})}` : 'Pagamento por Produção'}
Data de Admissão: ${employee.hireDate}
Tipo de Contrato: ${employee.contractType || 'Não informado'}
Status: ${employee.status}

💳 DADOS BANCÁRIOS:
Banco: ${employee.bank || 'Não informado'}
Agência/Conta: ${employee.bankAccount || 'Não informado'}

🚨 CONTATO DE EMERGÊNCIA:
Nome: ${employee.emergencyContact || 'Não informado'}
Telefone: ${employee.emergencyPhone || 'Não informado'}

📝 OBSERVAÇÕES:
${employee.notes || 'Nenhuma observação'}

${employee.status === 'demitido' && employee.dismissalDate ? `
❌ DEMISSÃO:
Data da Demissão: ${employee.dismissalDate}
Motivo: ${employee.dismissalReason || 'Não informado'}
` : ''}
                `;
                
                alert(details);
            }
        }

        function dismissEmployee(id) {
            const employee = employees.find(e => e.id === id);
            if (employee && employee.status === 'ativo') {
                const dismissalDate = prompt('Data da demissão (DD/MM/AAAA):', new Date().toLocaleDateString('pt-BR'));
                if (dismissalDate) {
                    const reason = prompt('Motivo da demissão (opcional):', '');
                    
                    employee.status = 'demitido';
                    employee.dismissalDate = dismissalDate;
                    employee.dismissalReason = reason;
                    
                    renderEmployees();
                    updateEmployeeSummary();
                    updatePayrollEmployeeSelect();
                    
                    alert(`Funcionário ${employee.name} foi demitido em ${dismissalDate}`);
                }
            }
        }

        function confirmDeleteEmployee(id) {
            const employee = employees.find(e => e.id === id);
            if (!employee) return;
            
            // Create confirmation modal
            const modal = document.createElement('div');
            modal.className = 'fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center z-50 p-4';
            modal.innerHTML = `
                <div class="bg-white rounded-xl shadow-lg max-w-md w-full p-6">
                    <div class="text-center">
                        <div class="mx-auto flex items-center justify-center h-12 w-12 rounded-full bg-red-100 mb-4">
                            <svg class="h-6 w-6 text-red-600" fill="currentColor" viewBox="0 0 24 24">
                                <path d="M6 19c0 1.1.9 2 2 2h8c1.1 0 2-.9 2-2V7H6v12zM19 4h-3.5l-1-1h-5l-1 1H5v2h14V4z"/>
                            </svg>
                        </div>
                        <h3 class="text-lg font-medium text-gray-900 mb-2">Excluir Funcionário</h3>
                        <p class="text-sm text-gray-500 mb-6">
                            Tem certeza que deseja excluir permanentemente <strong>${employee.name}</strong> do sistema?
                            <br><br>
                            <span class="text-red-600 font-medium">⚠️ Esta ação não pode ser desfeita!</span>
                            <br><br>
                            Todos os dados do funcionário, incluindo histórico de pagamentos, serão removidos.
                            ${employee.status === 'ativo' ? '<br><br><span class="text-yellow-600">💡 Dica: Se o funcionário ainda trabalha na empresa, considere usar "Demitir" ao invés de excluir.</span>' : ''}
                        </p>
                        <div class="flex space-x-3">
                            <button onclick="closeDeleteModal()" class="flex-1 px-4 py-2 text-gray-600 border border-gray-300 rounded-lg hover:bg-gray-50">
                                Cancelar
                            </button>
                            <button onclick="deleteEmployeePermanently(${id})" class="flex-1 px-4 py-2 bg-red-600 text-white rounded-lg hover:bg-red-700">
                                Excluir Permanentemente
                            </button>
                        </div>
                    </div>
                </div>
            `;
            
            document.body.appendChild(modal);
        }
        
        function closeDeleteModal() {
            const modal = document.querySelector('.fixed.inset-0');
            if (modal) {
                modal.remove();
            }
        }
        
        function deleteEmployeePermanently(id) {
            const employee = employees.find(e => e.id === id);
            if (employee) {
                // Remove employee
                employees = employees.filter(emp => emp.id !== id);
                
                // Remove related payroll records
                payrollRecords = payrollRecords.filter(payroll => payroll.employeeId != id);
                
                // Update displays
                renderEmployees();
                renderPayrollHistory();
                updateEmployeeSummary();
                updatePayrollEmployeeSelect();
                updateReminders();
                
                closeDeleteModal();
                alert(`Funcionário ${employee.name} foi excluído permanentemente do sistema.`);
            }
        }

        function updateEmployeeSummary() {
            const activeEmployees = employees.filter(e => e.status === 'ativo').length;
            const monthlyPayroll = employees
                .filter(e => e.status === 'ativo' && e.salary > 0)
                .reduce((sum, e) => sum + e.salary, 0);
            
            const productionEmployees = employees.filter(e => e.status === 'ativo' && e.salary === 0).length;
            
            document.getElementById('totalEmployees').textContent = activeEmployees;
            
            let payrollText = `R$ ${monthlyPayroll.toLocaleString('pt-BR', {minimumFractionDigits: 2})}`;
            if (productionEmployees > 0) {
                payrollText += ` + ${productionEmployees} por produção`;
            }
            
            document.getElementById('monthlyPayroll').textContent = payrollText;
        }

        function updatePayrollEmployeeSelect() {
            const select = document.getElementById('payrollEmployee');
            select.innerHTML = '<option value="">Selecione um funcionário</option>';
            
            employees.filter(e => e.status === 'ativo').forEach(employee => {
                const option = document.createElement('option');
                option.value = employee.id;
                option.textContent = `${employee.name} - ${employee.role}`;
                select.appendChild(option);
            });
        }

        // Production tracking functions
        function addProductionRecord() {
            const employeeId = document.getElementById('productionEmployee').value;
            const date = document.getElementById('productionDate').value;
            const quantity = parseFloat(document.getElementById('productionQuantity').value);
            const sector = document.getElementById('productionSector').value;
            const hours = parseFloat(document.getElementById('productionHours').value);
            const notes = document.getElementById('productionNotes').value;
            
            if (!employeeId || !date || !quantity) {
                alert('Por favor, preencha funcionário, data e quantidade');
                return;
            }
            
            const employee = employees.find(e => e.id == employeeId);
            if (!employee) {
                alert('Funcionário não encontrado');
                return;
            }
            
            const record = {
                id: Date.now(),
                employeeId: employeeId,
                employeeName: employee.name,
                date: date,
                dateFormatted: new Date(date).toLocaleDateString('pt-BR'),
                quantity: quantity,
                sector: sector || '',
                hours: hours || 0,
                notes: notes || '',
                addedAt: new Date().toISOString()
            };
            
            productionRecords.push(record);
            renderProductionRecords();
            updateProductionSummary();
            updateProductionEmployeeSelects();
            
            // Clear form
            document.getElementById('productionEmployee').value = '';
            document.getElementById('productionQuantity').value = '';
            document.getElementById('productionSector').value = '';
            document.getElementById('productionHours').value = '';
            document.getElementById('productionNotes').value = '';
            
            alert(`Produção de ${quantity} sacas registrada para ${employee.name}!`);
        }
        
        function renderProductionRecords() {
            const container = document.getElementById('productionRecordsList');
            container.innerHTML = '';
            
            const filteredRecords = filterProductionRecordsArray();
            
            if (filteredRecords.length === 0) {
                container.innerHTML = '<p class="text-gray-500 text-sm">Nenhum registro encontrado</p>';
                return;
            }
            
            const sortedRecords = filteredRecords.sort((a, b) => new Date(b.date) - new Date(a.date));
            
            sortedRecords.forEach(record => {
                const div = document.createElement('div');
                div.className = 'bg-blue-50 p-3 rounded-lg border-l-4 border-blue-400';
                div.innerHTML = `
                    <div class="flex justify-between items-start">
                        <div class="flex-1">
                            <p class="font-medium">${record.employeeName} - ${record.quantity} sacas</p>
                            <p class="text-sm text-gray-600">${record.dateFormatted}${record.sector ? ` | ${record.sector}` : ''}${record.hours ? ` | ${record.hours}h` : ''}</p>
                            ${record.notes ? `<p class="text-sm text-gray-500 italic mt-1">${record.notes}</p>` : ''}
                        </div>
                        <div class="flex space-x-2">
                            <button onclick="editProductionRecord(${record.id})" class="text-blue-600 hover:text-blue-800" title="Editar">
                                <svg class="w-4 h-4" fill="currentColor" viewBox="0 0 24 24">
                                    <path d="M3 17.25V21h3.75L17.81 9.94l-3.75-3.75L3 17.25zM20.71 7.04c.39-.39.39-1.02 0-1.41l-2.34-2.34c-.39-.39-1.02-.39-1.41 0l-1.83 1.83 3.75 3.75 1.83-1.83z"/>
                                </svg>
                            </button>
                            <button onclick="removeProductionRecord(${record.id})" class="text-red-600 hover:text-red-800" title="Excluir">
                                <svg class="w-4 h-4" fill="currentColor" viewBox="0 0 24 24">
                                    <path d="M19 6.41L17.59 5 12 10.59 6.41 5 5 6.41 10.59 12 5 17.59 6.41 19 12 13.41 17.59 19 19 17.59 13.41 12z"/>
                                </svg>
                            </button>
                        </div>
                    </div>
                `;
                container.appendChild(div);
            });
        }
        
        function filterProductionRecordsArray() {
            const employeeFilter = document.getElementById('productionFilterEmployee').value;
            const periodFilter = document.getElementById('productionFilterPeriod').value;
            const today = new Date();
            
            return productionRecords.filter(record => {
                const employeeMatch = employeeFilter === 'all' || record.employeeId == employeeFilter;
                
                let periodMatch = true;
                const recordDate = new Date(record.date);
                
                if (periodFilter === 'week') {
                    const weekAgo = new Date(today);
                    weekAgo.setDate(weekAgo.getDate() - 7);
                    periodMatch = recordDate >= weekAgo;
                } else if (periodFilter === 'month') {
                    const monthAgo = new Date(today);
                    monthAgo.setMonth(monthAgo.getMonth() - 1);
                    periodMatch = recordDate >= monthAgo;
                }
                
                return employeeMatch && periodMatch;
            });
        }
        
        function filterProductionRecords() {
            renderProductionRecords();
        }
        
        function editProductionRecord(id) {
            const record = productionRecords.find(r => r.id === id);
            if (!record) return;
            
            const newQuantity = parseFloat(prompt('Nova quantidade (sacas):', record.quantity));
            if (newQuantity && newQuantity > 0) {
                record.quantity = newQuantity;
                const newNotes = prompt('Observações:', record.notes || '');
                record.notes = newNotes || '';
                
                renderProductionRecords();
                updateProductionSummary();
                alert('Registro atualizado com sucesso!');
            }
        }
        
        function removeProductionRecord(id) {
            if (confirm('Tem certeza que deseja excluir este registro de produção?')) {
                productionRecords = productionRecords.filter(record => record.id !== id);
                renderProductionRecords();
                updateProductionSummary();
            }
        }
        
        function updateProductionSummary() {
            const today = new Date().toDateString();
            const todayProduction = productionRecords
                .filter(record => new Date(record.date).toDateString() === today)
                .reduce((sum, record) => sum + record.quantity, 0);
            
            const weekAgo = new Date();
            weekAgo.setDate(weekAgo.getDate() - 7);
            const weekProduction = productionRecords
                .filter(record => new Date(record.date) >= weekAgo)
                .reduce((sum, record) => sum + record.quantity, 0);
            
            document.getElementById('todayProduction').textContent = `${todayProduction} sacas`;
            document.getElementById('weekProduction').textContent = `${weekProduction} sacas`;
        }
        
        function updateProductionEmployeeSelects() {
            const productionSelect = document.getElementById('productionEmployee');
            const filterSelect = document.getElementById('productionFilterEmployee');
            
            // Update production form select
            productionSelect.innerHTML = '<option value="">Selecione um funcionário</option>';
            employees.filter(e => e.status === 'ativo').forEach(employee => {
                const option = document.createElement('option');
                option.value = employee.id;
                option.textContent = `${employee.name} - ${employee.role}`;
                productionSelect.appendChild(option);
            });
            
            // Update filter select
            filterSelect.innerHTML = '<option value="all">Todos os funcionários</option>';
            employees.forEach(employee => {
                const option = document.createElement('option');
                option.value = employee.id;
                option.textContent = employee.name;
                filterSelect.appendChild(option);
            });
        }

        // Payroll management functions
        function togglePaymentFields() {
            const type = document.getElementById('payrollType').value;
            const fixedFields = document.getElementById('fixedPaymentFields');
            const accumulatedFields = document.getElementById('accumulatedProductionFields');
            const customFields = document.getElementById('customPeriodFields');
            
            if (type === 'producao-acumulada') {
                fixedFields.classList.add('hidden');
                accumulatedFields.classList.remove('hidden');
                
                // Show/hide custom period fields
                const period = document.getElementById('productionPeriod').value;
                if (period === 'custom') {
                    customFields.classList.remove('hidden');
                } else {
                    customFields.classList.add('hidden');
                }
            } else {
                fixedFields.classList.remove('hidden');
                accumulatedFields.classList.add('hidden');
                customFields.classList.add('hidden');
            }
        }
        
        function loadEmployeeProduction() {
            const employeeId = document.getElementById('payrollEmployee').value;
            if (employeeId && document.getElementById('payrollType').value === 'producao-acumulada') {
                calculateAccumulatedProduction();
            }
        }
        
        function calculateAccumulatedProduction() {
            const employeeId = document.getElementById('payrollEmployee').value;
            const period = document.getElementById('productionPeriod').value;
            const pricePerBag = parseFloat(document.getElementById('accumulatedPricePerBag').value) || 0;
            
            if (!employeeId) return;
            
            let startDate, endDate;
            const today = new Date();
            
            if (period === 'custom') {
                const customStart = document.getElementById('customStartDate').value;
                const customEnd = document.getElementById('customEndDate').value;
                if (!customStart || !customEnd) return;
                
                startDate = new Date(customStart);
                endDate = new Date(customEnd);
            } else {
                endDate = new Date(today);
                startDate = new Date(today);
                
                if (period === 'week') {
                    startDate.setDate(startDate.getDate() - 7);
                } else if (period === 'biweekly') {
                    startDate.setDate(startDate.getDate() - 14);
                } else if (period === 'month') {
                    startDate.setMonth(startDate.getMonth() - 1);
                }
            }
            
            const employeeProduction = productionRecords.filter(record => 
                record.employeeId == employeeId &&
                new Date(record.date) >= startDate &&
                new Date(record.date) <= endDate
            );
            
            const totalBags = employeeProduction.reduce((sum, record) => sum + record.quantity, 0);
            const workingDays = new Set(employeeProduction.map(record => record.date)).size;
            const totalAmount = totalBags * pricePerBag;
            
            document.getElementById('accumulatedBags').textContent = totalBags.toFixed(1);
            document.getElementById('workingDays').textContent = workingDays;
            document.getElementById('accumulatedTotal').textContent = `R$ ${totalAmount.toLocaleString('pt-BR', {minimumFractionDigits: 2})}`;
        }
        
        // Add event listener for production period changes
        document.addEventListener('DOMContentLoaded', function() {
            const productionPeriodSelect = document.getElementById('productionPeriod');
            if (productionPeriodSelect) {
                productionPeriodSelect.addEventListener('change', function() {
                    const customFields = document.getElementById('customPeriodFields');
                    if (this.value === 'custom') {
                        customFields.classList.remove('hidden');
                    } else {
                        customFields.classList.add('hidden');
                    }
                    calculateAccumulatedProduction();
                });
            }
        });

        function addPayroll() {
            const employeeId = document.getElementById('payrollEmployee').value;
            const type = document.getElementById('payrollType').value;
            const reference = document.getElementById('payrollReference').value;
            
            let amount, date, bags, pricePerBag, period, workingDays;
            
            if (type === 'producao-acumulada') {
                bags = parseFloat(document.getElementById('accumulatedBags').textContent);
                pricePerBag = parseFloat(document.getElementById('accumulatedPricePerBag').value);
                amount = parseFloat(document.getElementById('accumulatedTotal').textContent.replace('R$ ', '').replace(/\./g, '').replace(',', '.'));
                date = document.getElementById('accumulatedPaymentDate').value;
                period = document.getElementById('productionPeriod').value;
                workingDays = parseInt(document.getElementById('workingDays').textContent);
                
                if (!bags || !pricePerBag || !date || bags === 0) {
                    alert('Por favor, selecione um funcionário, defina o valor por saca e verifique se há produção no período');
                    return;
                }
            } else {
                amount = parseFloat(document.getElementById('payrollAmount').value);
                date = document.getElementById('payrollDate').value;
                
                if (!amount || !date) {
                    alert('Por favor, preencha valor e data');
                    return;
                }
            }
            
            if (!employeeId) {
                alert('Por favor, selecione um funcionário');
                return;
            }
            
            const employee = employees.find(e => e.id == employeeId);
            if (!employee) {
                alert('Funcionário não encontrado');
                return;
            }
            
            const payroll = {
                id: Date.now(),
                employeeId: employeeId,
                employeeName: employee.name,
                type: type,
                amount: amount,
                date: new Date(date).toLocaleDateString('pt-BR'),
                reference: reference,
                bags: bags || null,
                pricePerBag: pricePerBag || null,
                period: period || null,
                workingDays: workingDays || null,
                addedAt: new Date().toISOString()
            };
            
            payrollRecords.push(payroll);
            renderPayrollHistory();
            
            // Add to expenses
            const expenseDescription = type === 'producao-acumulada' 
                ? `Pagamento por Produção - ${employee.name} (${bags.toFixed(1)} sacas em ${workingDays} dias)`
                : `Pagamento - ${employee.name} (${type})`;
                
            const expense = {
                id: Date.now() + 1,
                type: 'expense',
                description: expenseDescription,
                amount: amount,
                category: 'mao-obra',
                date: new Date(date).toLocaleDateString('pt-BR')
            };
            expenses.push(expense);
            updateFinancialSummary();
            
            // Clear form
            document.getElementById('payrollEmployee').value = '';
            document.getElementById('payrollReference').value = '';
            
            if (type === 'producao-acumulada') {
                document.getElementById('accumulatedPricePerBag').value = '';
                document.getElementById('accumulatedBags').textContent = '0';
                document.getElementById('workingDays').textContent = '0';
                document.getElementById('accumulatedTotal').textContent = 'R$ 0,00';
                document.getElementById('accumulatedPaymentDate').value = '';
            } else {
                document.getElementById('payrollAmount').value = '';
                document.getElementById('payrollDate').value = '';
            }
            
            // Reset to fixed payment fields
            document.getElementById('payrollType').value = 'salario';
            togglePaymentFields();
            
            alert(`Pagamento de R$ ${amount.toLocaleString('pt-BR', {minimumFractionDigits: 2})} registrado para ${employee.name}!`);
        }

        function renderPayrollHistory() {
            const container = document.getElementById('payrollHistory');
            container.innerHTML = '';
            
            if (payrollRecords.length === 0) {
                container.innerHTML = '<p class="text-gray-500 text-sm">Nenhum pagamento registrado ainda</p>';
                return;
            }
            
            const sortedPayrolls = payrollRecords.sort((a, b) => 
                new Date(b.date.split('/').reverse().join('-')) - new Date(a.date.split('/').reverse().join('-'))
            );
            
            sortedPayrolls.slice(0, 10).forEach(payroll => {
                const div = document.createElement('div');
                const isAccumulatedProduction = payroll.type === 'producao-acumulada';
                const isOldProduction = payroll.type === 'producao';
                const isProduction = isAccumulatedProduction || isOldProduction;
                
                div.className = `${isProduction ? 'bg-yellow-50 border-l-4 border-yellow-400' : 'bg-green-50'} p-3 rounded-lg`;
                
                let detailsHtml = '';
                if (isAccumulatedProduction && payroll.bags && payroll.pricePerBag) {
                    detailsHtml = `
                        <div class="text-xs text-gray-600 mt-1">
                            <span class="bg-yellow-100 px-2 py-1 rounded">☕ ${payroll.bags.toFixed(1)} sacas × R$ ${payroll.pricePerBag.toFixed(2)}</span>
                            ${payroll.workingDays ? `<span class="ml-2 bg-blue-100 px-2 py-1 rounded">📅 ${payroll.workingDays} dias</span>` : ''}
                            ${payroll.period ? `<span class="ml-2 text-gray-500">(${payroll.period === 'week' ? 'Semana' : payroll.period === 'biweekly' ? '2 Semanas' : payroll.period === 'month' ? 'Mês' : 'Personalizado'})</span>` : ''}
                        </div>
                    `;
                } else if (isOldProduction && payroll.bags && payroll.pricePerBag) {
                    detailsHtml = `
                        <div class="text-xs text-gray-600 mt-1">
                            <span class="bg-yellow-100 px-2 py-1 rounded">☕ ${payroll.bags} sacas × R$ ${payroll.pricePerBag.toFixed(2)}</span>
                            ${payroll.harvestPeriod ? `<span class="ml-2">📅 ${payroll.harvestPeriod}</span>` : ''}
                        </div>
                    `;
                }
                
                const paymentTypeLabel = isAccumulatedProduction ? 'Produção Acumulada' : 
                                       isOldProduction ? 'Produção Diária' : 
                                       payroll.type;
                
                div.innerHTML = `
                    <div class="flex justify-between items-start">
                        <div class="flex-1">
                            <p class="font-medium">${payroll.employeeName} - ${paymentTypeLabel}</p>
                            <p class="text-sm text-gray-600">${payroll.date}${payroll.reference ? ` | ${payroll.reference}` : ''}</p>
                            ${detailsHtml}
                        </div>
                        <div class="text-right">
                            <p class="font-bold ${isProduction ? 'text-yellow-600' : 'text-green-600'}">R$ ${payroll.amount.toLocaleString('pt-BR', {minimumFractionDigits: 2})}</p>
                            ${isProduction ? '<span class="text-xs bg-yellow-200 text-yellow-800 px-2 py-1 rounded-full">Produção</span>' : ''}
                        </div>
                    </div>
                `;
                container.appendChild(div);
            });
        }

        // Farm settings functions
        function loadFarmSettings() {
            document.getElementById('farmNameInput').value = farmSettings.name;
            document.getElementById('farmOwner').value = farmSettings.owner;
            document.getElementById('farmLocation').value = farmSettings.location;
            document.getElementById('farmTotalArea').value = farmSettings.totalArea;
            document.getElementById('farmAltitude').value = farmSettings.altitude;
            document.getElementById('farmMainCoffee').value = farmSettings.mainCoffee;
            document.getElementById('farmNotes').value = farmSettings.notes;
            
            // Update header
            document.getElementById('farmName').textContent = farmSettings.name;
        }

        function saveFarmSettings() {
            farmSettings.name = document.getElementById('farmNameInput').value || 'Minha Propriedade';
            farmSettings.owner = document.getElementById('farmOwner').value;
            farmSettings.location = document.getElementById('farmLocation').value;
            farmSettings.totalArea = parseFloat(document.getElementById('farmTotalArea').value) || 0;
            farmSettings.altitude = parseFloat(document.getElementById('farmAltitude').value) || 0;
            farmSettings.mainCoffee = document.getElementById('farmMainCoffee').value;
            farmSettings.notes = document.getElementById('farmNotes').value;
            
            // Update header
            document.getElementById('farmName').textContent = farmSettings.name;
            
            // Update dashboard if area was set
            if (farmSettings.totalArea > 0) {
                document.getElementById('totalArea').textContent = farmSettings.totalArea.toFixed(2);
            }
            
            alert('Configurações da fazenda salvas com sucesso!');
        }

        function saveSystemSettings() {
            alert('Configurações do sistema salvas com sucesso!');
            updateSystemStats();
        }

        function updateSystemStats() {
            document.getElementById('systemTaskCount').textContent = tasks.length;
            document.getElementById('systemInventoryCount').textContent = inventory.length;
            document.getElementById('systemEquipmentCount').textContent = equipment.length;
            document.getElementById('systemEmployeeCount').textContent = employees.length;
        }

        // Data management functions
        function exportData() {
            const data = {
                farmSettings: farmSettings,
                employees: employees,
                payrollRecords: payrollRecords,
                productionRecords: productionRecords,
                tasks: tasks,
                inventory: inventory,
                equipment: equipment,
                revenues: revenues,
                expenses: expenses,
                harvestRecords: harvestRecords,
                plantingRecords: plantingRecords,
                irrigationSchedules: irrigationSchedules,
                fertilizerSchedules: fertilizerSchedules,
                reminderSettings: reminderSettings,
                exportDate: new Date().toISOString()
            };
            
            const dataStr = JSON.stringify(data, null, 2);
            const dataBlob = new Blob([dataStr], {type: 'application/json'});
            const url = URL.createObjectURL(dataBlob);
            
            const link = document.createElement('a');
            link.href = url;
            link.download = `cafeplan-backup-${new Date().toISOString().split('T')[0]}.json`;
            link.click();
            
            URL.revokeObjectURL(url);
            alert('Dados exportados com sucesso!');
        }

        function importData() {
            const input = document.createElement('input');
            input.type = 'file';
            input.accept = '.json';
            input.onchange = function(e) {
                const file = e.target.files[0];
                if (file) {
                    const reader = new FileReader();
                    reader.onload = function(e) {
                        try {
                            const data = JSON.parse(e.target.result);
                            
                            // Import data
                            if (data.farmSettings) farmSettings = data.farmSettings;
                            if (data.employees) employees = data.employees;
                            if (data.payrollRecords) payrollRecords = data.payrollRecords;
                            if (data.productionRecords) productionRecords = data.productionRecords;
                            if (data.tasks) tasks = data.tasks;
                            if (data.inventory) inventory = data.inventory;
                            if (data.equipment) equipment = data.equipment;
                            if (data.revenues) revenues = data.revenues;
                            if (data.expenses) expenses = data.expenses;
                            if (data.harvestRecords) harvestRecords = data.harvestRecords;
                            if (data.plantingRecords) plantingRecords = data.plantingRecords;
                            if (data.irrigationSchedules) irrigationSchedules = data.irrigationSchedules;
                            if (data.fertilizerSchedules) fertilizerSchedules = data.fertilizerSchedules;
                            if (data.reminderSettings) reminderSettings = data.reminderSettings;
                            
                            // Refresh all displays
                            loadFarmSettings();
                            renderEmployees();
                            renderPayrollHistory();
                            renderProductionRecords();
                            updateEmployeeSummary();
                            updatePayrollEmployeeSelect();
                            updateProductionEmployeeSelects();
                            updateProductionSummary();
                            renderTasks();
                            renderInventory();
                            renderEquipment();
                            updateFinancialSummary();
                            updateDashboard();
                            updateReminders();
                            
                            alert('Dados importados com sucesso!');
                        } catch (error) {
                            alert('Erro ao importar dados. Verifique se o arquivo está correto.');
                        }
                    };
                    reader.readAsText(file);
                }
            };
            input.click();
        }

        function clearAllData() {
            if (confirm('ATENÇÃO: Esta ação irá apagar todos os dados do sistema. Esta operação não pode ser desfeita. Tem certeza?')) {
                if (confirm('Última confirmação: Todos os dados serão perdidos permanentemente. Continuar?')) {
                    // Clear all data
                    employees = [];
                    payrollRecords = [];
                    productionRecords = [];
                    tasks = [];
                    inventory = [];
                    equipment = [];
                    revenues = [];
                    expenses = [];
                    harvestRecords = [];
                    plantingRecords = [];
                    irrigationSchedules = [];
                    fertilizerSchedules = [];
                    reminders = [];
                    farmSettings = {
                        name: 'Minha Propriedade',
                        owner: '',
                        location: '',
                        totalArea: 0,
                        altitude: 0,
                        mainCoffee: 'arabica',
                        notes: ''
                    };
                    
                    // Refresh all displays
                    loadFarmSettings();
                    renderEmployees();
                    renderPayrollHistory();
                    renderProductionRecords();
                    updateEmployeeSummary();
                    updatePayrollEmployeeSelect();
                    updateProductionEmployeeSelects();
                    updateProductionSummary();
                    renderTasks();
                    renderInventory();
                    renderEquipment();
                    updateFinancialSummary();
                    updateDashboard();
                    updateReminders();
                    
                    alert('Todos os dados foram limpos com sucesso!');
                }
            }
        }

        // Reminder System Functions
        function generateReminders() {
            reminders = [];
            const today = new Date();
            
            // Payroll reminders (every 5th of the month)
            if (reminderSettings.payrollReminder) {
                const payrollDate = new Date(today.getFullYear(), today.getMonth(), 5);
                if (payrollDate <= today) {
                    payrollDate.setMonth(payrollDate.getMonth() + 1);
                }
                
                const daysUntilPayroll = Math.ceil((payrollDate - today) / (1000 * 60 * 60 * 24));
                if (daysUntilPayroll <= 3) {
                    reminders.push({
                        id: 'payroll-' + payrollDate.getTime(),
                        type: 'payroll',
                        priority: 'high',
                        title: 'Pagamento de Funcionários',
                        message: `Pagamento da folha deve ser feito em ${daysUntilPayroll} dias (${payrollDate.toLocaleDateString('pt-BR')})`,
                        date: payrollDate,
                        action: () => showTab('employees')
                    });
                }
            }
            
            // Task reminders
            if (reminderSettings.taskReminder) {
                const overdueTasks = tasks.filter(task => 
                    !task.completed && new Date(task.date) < today
                );
                
                const todayTasks = tasks.filter(task => 
                    !task.completed && 
                    new Date(task.date).toDateString() === today.toDateString()
                );
                
                if (overdueTasks.length > 0) {
                    reminders.push({
                        id: 'overdue-tasks',
                        type: 'task',
                        priority: 'high',
                        title: 'Tarefas Atrasadas',
                        message: `${overdueTasks.length} tarefa(s) atrasada(s) precisam de atenção`,
                        action: () => showTab('tasks')
                    });
                }
                
                if (todayTasks.length > 0) {
                    reminders.push({
                        id: 'today-tasks',
                        type: 'task',
                        priority: 'medium',
                        title: 'Tarefas de Hoje',
                        message: `${todayTasks.length} tarefa(s) programada(s) para hoje`,
                        action: () => showTab('tasks')
                    });
                }
            }
            
            // Equipment maintenance reminders
            if (reminderSettings.maintenanceReminder) {
                const maintenanceNeeded = equipment.filter(item => 
                    item.hours >= item.nextMaintenance && item.nextMaintenance > 0
                );
                
                if (maintenanceNeeded.length > 0) {
                    reminders.push({
                        id: 'maintenance-needed',
                        type: 'maintenance',
                        priority: 'high',
                        title: 'Manutenção de Equipamentos',
                        message: `${maintenanceNeeded.length} equipamento(s) precisam de manutenção`,
                        action: () => showTab('equipment')
                    });
                }
            }
            
            // Stock reminders
            if (reminderSettings.stockReminder) {
                const lowStockItems = inventory.filter(item => item.quantity <= item.minStock);
                
                if (lowStockItems.length > 0) {
                    reminders.push({
                        id: 'low-stock',
                        type: 'stock',
                        priority: 'medium',
                        title: 'Estoque Baixo',
                        message: `${lowStockItems.length} item(ns) com estoque baixo`,
                        action: () => showTab('inventory')
                    });
                }
            }
            
            // Harvest season reminders (May to September)
            if (reminderSettings.harvestReminder) {
                const currentMonth = today.getMonth() + 1;
                if (currentMonth >= 5 && currentMonth <= 9) {
                    reminders.push({
                        id: 'harvest-season',
                        type: 'harvest',
                        priority: 'medium',
                        title: 'Época de Colheita',
                        message: 'Estamos na época de colheita do café. Monitore a maturação dos frutos',
                        action: () => showTab('harvest')
                    });
                }
            }
            
            // Irrigation schedule reminders
            if (reminderSettings.irrigationReminder) {
                const todayIrrigation = irrigationSchedules.filter(schedule => {
                    const scheduleTime = new Date();
                    const [hours, minutes] = schedule.time.split(':');
                    scheduleTime.setHours(parseInt(hours), parseInt(minutes), 0, 0);
                    
                    const now = new Date();
                    const timeDiff = scheduleTime - now;
                    return timeDiff > 0 && timeDiff <= 3600000; // Next hour
                });
                
                if (todayIrrigation.length > 0) {
                    reminders.push({
                        id: 'irrigation-today',
                        type: 'irrigation',
                        priority: 'medium',
                        title: 'Irrigação Programada',
                        message: `${todayIrrigation.length} irrigação(ões) programada(s) para a próxima hora`,
                        action: () => showTab('irrigation')
                    });
                }
            }
            
            // Fertilizer schedule reminders
            if (reminderSettings.fertilizerReminder) {
                const upcomingFertilizer = fertilizerSchedules.filter(schedule => {
                    const scheduleDate = new Date(schedule.date.split('/').reverse().join('-'));
                    const daysUntil = Math.ceil((scheduleDate - today) / (1000 * 60 * 60 * 24));
                    return daysUntil >= 0 && daysUntil <= 2;
                });
                
                if (upcomingFertilizer.length > 0) {
                    reminders.push({
                        id: 'fertilizer-upcoming',
                        type: 'fertilizer',
                        priority: 'medium',
                        title: 'Adubação Programada',
                        message: `${upcomingFertilizer.length} adubação(ões) programada(s) para os próximos 2 dias`,
                        action: () => showTab('fertilizer')
                    });
                }
            }
            
            // Employee vacation reminders
            if (reminderSettings.vacationReminder) {
                const activeEmployees = employees.filter(e => e.status === 'ativo');
                const vacationDue = activeEmployees.filter(employee => {
                    const hireDate = new Date(employee.hireDate.split('/').reverse().join('-'));
                    const monthsSinceHire = (today - hireDate) / (1000 * 60 * 60 * 24 * 30);
                    return monthsSinceHire >= 12; // 1 year of work
                });
                
                if (vacationDue.length > 0) {
                    reminders.push({
                        id: 'vacation-due',
                        type: 'vacation',
                        priority: 'low',
                        title: 'Férias Pendentes',
                        message: `${vacationDue.length} funcionário(s) com direito a férias`,
                        action: () => showTab('employees')
                    });
                }
            }
            
            // Contract expiration reminders (for temporary employees)
            if (reminderSettings.contractReminder) {
                const temporaryEmployees = employees.filter(e => 
                    e.contractType === 'temporario' && e.status === 'ativo'
                );
                
                if (temporaryEmployees.length > 0) {
                    reminders.push({
                        id: 'contract-expiration',
                        type: 'contract',
                        priority: 'medium',
                        title: 'Contratos Temporários',
                        message: `${temporaryEmployees.length} contrato(s) temporário(s) para revisar`,
                        action: () => showTab('employees')
                    });
                }
            }
        }
        
        function updateReminders() {
            generateReminders();
            renderReminders();
        }
        
        function renderReminders() {
            const container = document.getElementById('remindersList');
            container.innerHTML = '';
            
            if (reminders.length === 0) {
                container.innerHTML = '<p class="text-gray-500 text-sm">✅ Nenhum lembrete pendente</p>';
                return;
            }
            
            // Sort by priority
            const priorityOrder = { 'high': 3, 'medium': 2, 'low': 1 };
            const sortedReminders = reminders.sort((a, b) => 
                priorityOrder[b.priority] - priorityOrder[a.priority]
            );
            
            sortedReminders.forEach(reminder => {
                const div = document.createElement('div');
                const priorityColors = {
                    'high': 'bg-red-50 border-l-4 border-red-400 text-red-800',
                    'medium': 'bg-yellow-50 border-l-4 border-yellow-400 text-yellow-800',
                    'low': 'bg-blue-50 border-l-4 border-blue-400 text-blue-800'
                };
                
                const icons = {
                    'payroll': '💰',
                    'task': '✅',
                    'maintenance': '🔧',
                    'stock': '📦',
                    'harvest': '☕',
                    'irrigation': '💧',
                    'fertilizer': '🌱',
                    'vacation': '🏖️',
                    'contract': '📄'
                };
                
                div.className = `p-3 rounded-lg ${priorityColors[reminder.priority]} cursor-pointer hover:opacity-80 transition-opacity`;
                div.onclick = reminder.action;
                div.innerHTML = `
                    <div class="flex items-start justify-between">
                        <div class="flex items-start space-x-2">
                            <span class="text-lg">${icons[reminder.type] || '🔔'}</span>
                            <div>
                                <p class="font-medium text-sm">${reminder.title}</p>
                                <p class="text-xs opacity-90">${reminder.message}</p>
                            </div>
                        </div>
                        <button onclick="dismissReminder('${reminder.id}'); event.stopPropagation();" class="text-xs opacity-60 hover:opacity-100">
                            ✕
                        </button>
                    </div>
                `;
                container.appendChild(div);
            });
        }
        
        function dismissReminder(id) {
            reminders = reminders.filter(reminder => reminder.id !== id);
            renderReminders();
        }
        
        function showReminderSettings() {
            showTab('settings');
            // Scroll to reminder settings
            setTimeout(() => {
                document.querySelector('#settings .bg-white:nth-child(3)').scrollIntoView({ 
                    behavior: 'smooth' 
                });
            }, 100);
        }
        
        function saveReminderSettings() {
            reminderSettings.payrollReminder = document.getElementById('payrollReminderSetting').checked;
            reminderSettings.taskReminder = document.getElementById('taskReminderSetting').checked;
            reminderSettings.maintenanceReminder = document.getElementById('maintenanceReminderSetting').checked;
            reminderSettings.stockReminder = document.getElementById('stockReminderSetting').checked;
            reminderSettings.harvestReminder = document.getElementById('harvestReminderSetting').checked;
            reminderSettings.irrigationReminder = document.getElementById('irrigationReminderSetting').checked;
            reminderSettings.fertilizerReminder = document.getElementById('fertilizerReminderSetting').checked;
            reminderSettings.contractReminder = document.getElementById('contractReminderSetting').checked;
            reminderSettings.vacationReminder = document.getElementById('vacationReminderSetting').checked;
            
            updateReminders();
            alert('Configurações de lembretes salvas com sucesso!');
        }
    </script>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'97b5fcf016f3f1c7',t:'MTc1NzI0NTgyMS4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
